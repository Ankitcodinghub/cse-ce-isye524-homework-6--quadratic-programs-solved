# cse-ce-isye524-homework-6--quadratic-programs-solved
**TO GET THIS SOLUTION VISIT:** [CSE-CE-ISyE524 Homework 6- Quadratic programs Solved](https://www.ankitcodinghub.com/product/cse-ce-isye524-homework-6-quadratic-programs-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;120328&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE-CE-ISyE524  Homework 6- Quadratic programs Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Submit pdf files via Canvas

1. Enclosing circle. Given a set of points in the plane xi ∈ R2, we would like to find the circle with smallest possible area that contains all of the points. Explain how to model this as an optimization problem. To test your model, generate a set of 50 random points using the code X = 4 .+ randn(2,50) (this generates a 2×50 matrix X whose columns are the xi). Produce a plot of the randomly generated points along with the enclosing circle of smallest area.

To get you started, the following Julia code generates the points and plots a circle:

using PyPlot

X = 4 .+ randn(2,50) # generate 50 random points

t = range(0,stop=2*3.141592654,length=100) # parameter that traverses the circle r = 2; x1 = 4; x2 = 4 # radius and coordinates of the center

plot( x1 .+ r*cos.(t), x2 .+ r*sin.(t)) # plot circle radius r with center (x1,x2) scatter( X[1,:], X[2,:], color=”black”) # plot the 50 points

axis(“equal”) # make x and y scales equal

2. Quadratic form positivity. You’re presented with the constraint:

2×2 + 2y2 + 9z2 + 8xy − 6xz − 6yz ≤ 1 (1) a) Write the constraint (1) in the standard form vTQv ≤ 1. Where Q is a symmetric matrix. What is Q and what is v?

b) It turns out the above constraint is not convex. In other words, the set of (x,y,z) satisfying the constraint (1) is not an ellipsoid. Explain why this is the case.

Note: you can perform an orthogonal decomposition of a symmetric matrix Q in Julia like this:

(Lambda,U) = eigen(Q) # Lambda is the vector of eigenvalues and U is orthogonal

U * diagm(Lambda) * U’ # this is equal to Q (as long as Q was symmetric to begin with)

c) We can also write the constraint (1) using norms by putting it in the form:

kAvk2−kBvk2 ≤ 1

What is v and what are the matrices A and B that make the constraint above equivalent to (1)?

d) Explain how to find (x,y,z) that satisfies the constraint (1) and that has arbitrarily large magnitude (i.e. x2 + y2 + z2 is as large as you like).

1 of 2

3. Lasso regression. Consider the data (x,y) plotted below, available in lasso_data.csv.

In this problem, we will investigate different approaches for performing polynomial regression.

a) Perform ordinary polynomial regression. Make plots that show the data as well as the best fit to the data for polynomials of degree d = 5 and d = 15. Also comment on the magnitudes of the coefficients in the resulting polynomial fits. Are they small or large?

b) In order to get smaller coefficients, we will use ridge regression (L2 regularization). Re-solve the d = 15 version of the problem using a regularization parameter λ = 10−6 and plot the new fit. How does the fit change compared to the non-regularized case of part a? How do the magnitudes of the coefficients in the resulting polynomial fit change?

2 of 2
