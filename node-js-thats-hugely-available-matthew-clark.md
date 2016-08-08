# Node.js that's hugely reliable, fast, and scalable - Matthew Clark, Jonathan Ishmael

[Original Video](https://www.youtube.com/watch?v=pxmXiKlh5OU&index=11&list=PL0CdgOSSGlBYnHAl_DZoy9BWvdVQjNKE2)

##  1.  Design as micro-services that embrace the elasticity of the cloud
  - Layers of Micro-services
  - Develop to be horizontally scalable
  - At least two for resilience
  - Replace unhealthy VMs
  - Scale upon demand
##  2.  Scale up like a rocket, down like a father
  - Scale is important, but knowing when to scale is difficult
  - What metrics should be used to decided when to scale?
    * There's no one-size-fits-all solution, it is dependends on your situation
    * Requires analysis, restudy and effort to get right
    * Being able to adapt quickly and in the right time
    * Still needs to be cost-effective
##  3.  Understand your load, in theory and for real
  - All architectures have weaknesses
  - Scaling the wrong thing may make the problem even bigger
    * e.g. Scaling web servers horizontally in a load balancer, while the source of slowness is the data-storage access.
##  4.  An event-drive approach helps scaling and load
  - Make your systems more efficient to keep scaling when the limits for scaling are hit
##  5.  Beware of the cost of micro-services
  - The financial cost of micro-services should be minimal
  - Many options and approaches
##  6.  It's fine to test your production environment
  - No matter how good you are, you will still have problems while testing
  - Sometimes it is not possible to catch problems outside production
  - Grow a good testing culture to help address those problems fast and improve it 
##  7.  Be two steps away from catastrophe
  - Make sure micro-services can handle it if one of them die
  - You cannot predict all situations
  - Always have a plan B to keep most part of the system running if some part of it has problems
  - Resilience is the word of the day
##  8.  Become great at running Node infrastructure
  - Running good infrastructure is as a big of a problem as building the system
  - Performant, efficient and reliable Node project is hard
  - Multi-disciplinary teams produce better solutions to the problems
  - Not just running PM2 or Nodemon, but system engineering and analysis is needed 
