jhc-06-morecolours
==================

This is a modified version of JHeatMap 0.6 by Tom Castle (www.tc33.org).

In this version, the colour change when the value increase, not only the brightness.
The colour scale used is:

     black->blue->green->yellow->red

That is, lower values are represented as black, highest as red.

Result
======
Example of resulting image (this is a test of an hash function)
![alt text](https://raw.github.com/jacopofar/jhc-06-morecolours/master/bloom_map.png "Result example")

Example usage
============
Just like the original version


    // Create some dummy data.
    double[][] data = new double[][]{{3,2,3,4,5,6},
                                     {2,3,4,5,6,7},
                                     {3,4,5,6,7,6},
                                     {4,5,6,7,6,5}};
    
    // Create our heat chart using our data.
    HeatChart chart = new HeatChart(data);
    
    // Customise the chart.
    chart.setTitle("This is my chart title");
    chart.setXAxisLabel("X Axis");
    chart.setYAxisLabel("Y Axis");
    
    // Output the chart to a file.
    chart.saveToFile(new File("my-chart.png"));



License
=======
As the original version, this software is released under GNU Lesser General Public License version 3, you cna find in in the attached file "LICENSE".
