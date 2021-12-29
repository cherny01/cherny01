- 👋 Hi, I’m @cherny01
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
cherny01/cherny01 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# step 1: read composite image
punks = Punks::Image::Composite.read( './punks.png' )

# step 2: mint all punks
(0..9999).each do |i|
  name = '%04d' % i
  punks[i].save( "./punk-#{name}.png" )
end
