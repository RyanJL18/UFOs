# UFOs
Filtering and interpreting data on UFO sightings around the United States.
## Overview
Using JavaScript and HTML we were tasked with creating a table filled with information about UFO Sightings. Along with this table presented on an HTML Page, we were tasked with being able to sift through the data and find corresponding values within the table using a filtered search bar. With this HTML Page in use, we can filter and compare a large number of sightings depending on the criteria input.
## Results
![Page_Screenshot.png](https://github.com/RyanJL18/UFOs/blob/main/Resources/Page%20Screenshot.png)

This was the result for the page that was created. As you can see, there is a heading with a background image, a description that gives insight as to the function of the table, and multiple search bars that offer the opportunity to narrow down search results with multiple inputs. This offers the opportunity to get very specific when looking into the presented data.

The Utility of these multiple search bars was made by creating a filter table in the HTML as follows:
```
<!-- Filter Table -->
      <div class="bg-dark container-fluid">
        <div class="row">
          <div class="col-md-3">
            <form class="bg-dark" action="">
                <p>Filter Search</p>
                <ul class="list-group bg-dark">
                  <!--Entered Value-->
                    <li class="list-group-item bg-dark">
                        <label for="date">Enter Date</label>
                        <input type="text" placeholder="1/1/2010" id="datetime" />
                    </li>
                    <li class="list-group-item bg-dark">
                        <label for="city">Enter City</label>
                        <input type="text" placeholder="roswell" id="city" />
                    </li>
                    <li class="list-group-item bg-dark">
                        <label for="state">Enter State</label>
                        <input type="text" placeholder="ca" id="state" />
                    </li>
                    <li class="list-group-item bg-dark">
                        <label for="country">Enter Country</label>
                        <input type="text" placeholder="us" id="country" />
                    </li>
                    <li class="list-group-item bg-dark">
                        <label for="shape">Enter Shape</label>
                        <input type="text" placeholder="circle" id="shape" />
                    </li>
                  <!-- <li class="list-group-item bg-dark">
                     <button id="filter-btn" type="button" class="btn btn-dark">
                       Filter Table
                     </button>
                  </li> -->
                </ul>
               </form>
          </div>
```

With this code, we created the search bar that functions with one or multiple inputs, narrowing down the data as more searches are used. As you can see with the examples below, using one search criteria like the shape offers an opportunity to compare entries with only one value in common, while adding values into both the state and country offers more specific results to compare.

![Search_Example.png](https://github.com/RyanJL18/UFOs/blob/main/Resources/Search%20Example.png)

![Search_Example2.png](https://github.com/RyanJL18/UFOs/blob/main/Resources/Search%20Example2.png)

## Final Thoughts
This ability to filter data in this way can be very useful! We were able to narrow down results based on multiple inputs and find entries with matching criteria that we could compare for further investigation into the question "Are UFO's Real?" However, this utility does have a couple drawbacks. One specific drawback that I ran into while testing was if your input did not match any of the entries, you would not receive any outputs. That is a success because it is exactly what we told the code to do but could be off putting to new users. This also only filters the data if it is written exactly as the value is written, which does cause for case sensitivity issues. A suggestion for rectifying this issue would be to potentially add a drop-down menu with the available options, so that new users could find entries with ease. Another potential quality of life improvement could be adding a "Similar Sightings" table below the search results that contains a few similar entries for easier comparison to more entries.

