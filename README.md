# Script
matriz

matrix(1:9,byrow=FALSE,nrow=3)

matrix(1:9,byrow=TRUE,nrow=3)

#Box office star wars(in millions!)
new_hope=c(460.998,314.4)
empire_strikes=c(290.475,247.900)
return_jedi=c(309.306,165.8)

#create box 
box_oficce=c(new_hope,empire_strikes,return_jedi)
box_oficce

#constructstar_wars_matrix#
star_wars_matrix=matrix(box_oficce,nrow=3,byrow=TRUE)
star_wars_matrix

#vectors region and titles, used for naming#
region=c("US","non_US")
region
titles=c("A new Hope","The Empire Strikes Back","Return of the Jedi")
titles

#name the column with region#
colnames(star_wars_matrix)=region

#namte the rows with titles#
rownames(star_wars_matrix)=titles

#print out star wars matrix#
star_wars_matrix

view(star_wars_matrix)


#Calculate worldwide box office figures#
worldwide_vector=rowSums(star_wars_matrix)
worldwide_vector

#Bind the new variable worldwide vector as column to star wars matrix#
all_wars_matrix=cbind(star_wars_matrix,worldwide_vector)
all_wars_matrix

all_wars_matrix=rbind(all_wars_matrix,all_wars_matrix2)
all_wars_matrix
