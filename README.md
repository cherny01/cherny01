- š Hi, Iām @cherny01
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
cherny01/cherny01 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# step 1: read composite image
punks = Punks::Image::Composite.read( './punks.png' )

# step 2: mint all punks
(0..9999).each do |i|
  name = '%04d' % i
  punks[i].save( "./punk-#{name}.png" )
end
