# assi7
vector
data <- c("Sun","Mon","Tue","Wed","Thurs","Fri","Sat")
data1 <- t[c(2,3,6)]
print(data1)
# Accessing vector elements using logical indexing.
data2<- t[c(TRUE,FALSE,FALSE,FALSE,FALSE,TRUE,FALSE)]
print(data2)
# Accessing vector elements using negative indexing.
data3 <- t[c(-2,-5)]
print(data3)
# Accessing vector elements using 0/1 indexing.
data4 <- t[c(0,0,0,0,0,0,1)]
print(data4)
output:
[1] "Mon" "Tue" "Fri"
[1] "Sun" "Fri"
[1] "Sun" "Tue" "Wed" "Fri" "Sat"
[1] "Sun"
#list
data4 <- list(c("Jan","Feb","Mar"), matrix(c(3,9,5,1,-2,8), nrow = 2),
 list("green",12.3))
names(data4) <- c("1st Quarter", "A_Matrix", "A Inner list")
print(data4)
output:
$`1st_Quarter`
[1] "Jan" "Feb" "Mar"
$A_Matrix
 [,1] [,2] [,3]
[1,] 3 5 -2
[2,] 9 1 8
$A_Inner_list
$A_Inner_list[[1]]
[1] "green"
$A_Inner_list[[2]]
[1] 12.3
#Matrix
example <- matrix(c(3:14), nrow = 4, byrow = TRUE)
print(M)
example2 <- matrix(c(3:14), nrow = 4, byrow = FALSE)
print(example2)
rownames = c("row1", "row2", "row3", "row4")
colnames = c("col1", "col2", "col3")
P3 <- matrix(c(3:14), nrow = 4, byrow = TRUE, dimnames = list(rownames, colnames))
print(P3)
Output:
[,1] [,2] [,3]
[1,] 3 4 5
[2,] 6 7 8
[3,] 9 10 11
[4,] 12 13 14
 [,1] [,2] [,3]
[1,] 3 7 11
[2,] 4 8 12
[3,] 5 9 13
[4,] 6 10 14
 col1 col2 col3
row1 3 4 5
row2 6 7 8
row3 9 10 11
row4 12 13 14
#factor
data <- c("East","West","East","North","North","East","West","West","West","East","North")
print(data)
output:
[1] "East" "West" "East" "North" "North" "East" "West" "West" "West" "East" "North"
#Graphs
ng(file = "boxplot.png")
boxplot(mpg ~ cyl, data = mtcars, xlab = "Number of Cylinders",ylab = "Miles Per Gallon", main = 
"Mileage Data")
dev.off()
data <- x(7,12,28,3,41)
# Give the chart file a name.
png(file = "line_chart.jpg")
plot(v,type = "o")
png(file = "boxplot.png")
boxplot(mpg ~ cyl, data = mtcars, xlab = "Number of Cylinders",
 ylab = "Miles Per Gallon", main = "Mileage Data")
dev.off()
dev.off()
#control strutre
new.function <- function(a) {
 for(i in 1:a) {
 b <- i^2
 print(b)
 }
}
new.function(6)

