<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Report</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
          text-align: center;
          color: #333;

        }
        .container {
      display: flex;
      justify-content: space-between;
      padding: 20px;
      background-color: #fff;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    .contact-info {
      width: 120%;
    }
    .social-links {
      width: 45%;
      display: flex;
      justify-content: space-around;
    }
    .social-links a {
      text-decoration: none;
      color: #333;
      font-size: 20px;
    }
    .company-logo {
      width: 45%;
      text-align: right;
    }
    .company-logo {
      text-align: center;
    }
    .company-logo img {
      max-width: 100%;
      height: auto;
      display: block; /* Center the image */
      margin: 0 auto; /* Center the image */
    }
  
    .github-link {
      display: flex;
      align-items: center;
      margin-top: 2px;
    }
    .github-link img {
      width: 30px;
      height: 30px;
      margin-right: 2px;
    }

    @media (max-width: 768px) {
            /* Adjustments for smaller screens */
            .container {
                flex-direction: column;
            }

            .contact-info,
            .company-logo {
                width: 100%;
            }

            .social-links {
                width: 100%;
            }

            /* Add more media query adjustments as needed */
        }


        h1 {
            color: #ffffff;
          background:linear-gradient(to right,#ffa201, #cd104d)
        }
      h2 {
      color: #15456a;
      margin: 0;
        background-color: #f0f0f0;
        text-align: left;

      }
      h3 {
        padding: 10px;
        margin: 5px;
      color: #15456a;
      margin: 0;
        text-align: left;

      }

      p {
          /* Light gray background */
          padding: 20px;
          margin: 10px;
        /* Add padding for better visual appeal */
          color: #333;
        text-align: justify;
        
      }
      
      table {
          width: 60%;
          border-collapse: collapse;
          margin-top: 10px;
        margin: auto
      }

      th, td {
          border: 1px solid #ddd;
          padding: 8px;
          text-align: left;
      }

      th {
          background-color: #3498db;
          color: #fff;
        text-align: justify;
      }
        </style>
</head>
<body>
  <div class="header">
    <h1>Netflix Report</h1>
    </div>
   <h2>Introduction</h2>
    <p>Netflix, the global entertainment giant, offers a vast array of movies and TV shows. This report focuses on a specific segment of Netflix data related to movies and TV shows. Our main objective is to leverage the combined capabilities of Pandas and NumPy. We aim to convert raw data into valuable insights, enabling a sophisticated analysis of trends across different variables. The goal is to uncover patterns that enhance our understanding of the dynamic landscape of Netflix content.</p>
  <h2>Methodology</h2>
  <p>The core methodology for this analysis centers on utilizing Pandas and NumPy functions. These tools are pivotal for cleaning and extracting pertinent information from the dataset. Sourced from the Kaggle community, the dataset serves as the foundation for our examination.</p>
  <h2>Data Overview</h2>
    <p>The dataset comprises 8,790 rows and 10 columns, offering a substantial volume of information for analysis. The columns encompass crucial details such as movie release names, dates, types, durations, and ratings. This structured arrangement provides a comprehensive snapshot, setting the stage for a detailed exploration of Netflix movies.</p>
  <h2>Key Features</h2>
  <table>
      <tr>
          <th>Name</th>
          <th>Role</th>
      </tr>
      <tr>
          <td>Data Cleaning</td>
          <td>Addressing data cleanliness, especially since only 1 of the 10 columns is numerical.</td>
      </tr>
      <tr>
          <td>Movie Type Analysis</td>
          <td>Counting and exploring different types of movies to understand variations.</td>
      </tr>
      <tr>
          <td>Director Information</td>
          <td>Identifying movies without director information, if any</td>
      </tr>
      <tr>
          <td>Country and Movie Type</td>
          <td>Grouping data by country and movie type to reveal patterns</td>
      </tr>
      <tr>
          <td>Top 10 Countries</td>
          <td>Selecting and prioritizing the top 10 countries with the most information</td>
      </tr>
      <tr>
          <td>Normal Distribution Analysis</td>
          <td>Exploring the normal distribution to understand the release year trends</td>
      </tr>
      <tr>
          <td>Data Transformation - Duration</td>
          <td>Transforming the duration variable, converting some entries from minutes to seasons.</td>
      </tr>
      <tr>
          <td>Category Splitting</td>
          <td>Splitting categories based on recommendations.</td>
      </tr>
      <tr>
          <td>Top 10 Categories</td>
          <td>Identifying and showcasing the top 10 categories based on analysis.</td>
      </tr>
      <tr>
          <td>Insights from Recommendations</td>
          <td>Extracting insights from the analysis of movie categories and recommendations.</td>
      </tr>

  </table>

  <h2>Data visualization</h2>
  <h3>Top 10 Countries by Movie Type</h3>
    <p>Visual representation showcasing the distribution of movie types in the top 10 countries.</p>
    <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/uno.png?raw=true" alt="Placeholder Image" style="max-width: 100%; height: auto;">
  <h3>Movie Ratings Analysis</h3>
  <p>Rating distribution visualization to discern patterns and trends in movie ratings.</p>
  <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/dos.png?raw=true"  alt="Placeholder Image" style="max-width: 100%">
  <h3>Seasons of Movies and TV Shows</h3>
  <p>Graphical exploration illustrating the distribution of movies and TV shows across different seasons.</p>
  <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/tres.png?raw=true"  alt="Placeholder Image" style="max-width: 100%">
  <h3>Top 10 Categories Distribution</h3>
  <p>Visual breakdown of the distribution of movies and TV shows across the top 10 categories.</p>
  <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/cuatro.png?raw=true"  alt="Placeholder Image" style="max-width: 100%">

  <h2>Trends and Patterns</h2>
  <table>
    <tr>
        <th>TV-MA Ratings Trend</th>
        <th>Preference for Single-Season Content</th>
        <th>Top 10 Categories Analysis</th>
    </tr>
    <tr>
        <td>Graphic representation revealing the trend of TV-MA ratings, with a notable frequency of 3205 instances. Valuable insights can be drawn from this pattern.</td>
        <td>After transforming the data to seasons, the analysis indicates a preference for shows or movies with a single season, with a total count of 1901. This trend sheds light on audience viewing habits.</td>
        <td>Exploration of the top 10 categories reveals that a significant portion of the content is dominated by international movies. This insight provides a glimpse into the diverse preferences of the audience.</td>
    </tr>
  </table>
  <h2>Challenges and Limitations</h2>
  <h3>Limited types in data</h3>
  <p>A limitation arises from the absence of certain types, such as sports, documentaries, and anime series. This gap impacts the comprehensiveness of the analysis, as these genres contribute distinct characteristics to Netflix content.</p>
  <h3>Content Availability by Country</h3>
  <p>The analysis acknowledges that content availability varies by country due to licensing restrictions imposed by Netflix. This factor introduces a level of contrast that can influence the overall analysis, particularly when considering regional preferences and restrictions.</p>
  <h3>Viewer engagement metrics absent</h3>
  <p>Another limitation stems from the absence of viewer engagement metrics, such as the number of views or user preferences. The lack of this variable restricts the analysis from gauging the popularity and audience preferences for each movie or TV show, which is crucial for a comprehensive understanding of Netflix content dynamics.</p>
  <h2>Recommendation</h2>
  <h3>Enhance Data Variety</h3>
  <p>Increase the diversity of data by incorporating additional types, such as sports, documentaries, and anime series. This will enrich the dataset, enabling a more comprehensive analysis.</p>
  <h3>Expand Variables</h3>
  <p>Consider adding more variables to the dataset to capture additional dimensions of user behavior, preferences, or content attributes. This expansion can provide deeper insights into the factors influencing viewership.</p>
  <h3>Utilize Predictive Analytics</h3>
  <p>Apply normal distribution graphics to relevant variables to identify patterns that may predict user choices. By leveraging predictive analytics, Netflix can gain valuable insights into viewer preferences, aiding in personalized content recommendations.</p>
  <h3>Explore Viewer Interaction Metrics</h3>
  <p>Integrate metrics related to viewer engagement, such as watch time, ratings, and user interactions. Understanding how users interact with content can unveil patterns and preferences that go beyond the current dataset limitations.</p>
  <h3>Collaborate for Viewer Surveys</h3>
  <p>Consider conducting viewer surveys to gather direct feedback on content preferences, allowing for a more nuanced understanding of audience tastes and expectations.</p>
  <h2>Conclusion</h2>
    <p>While this analysis offers valuable insights into Netflix content, limitations such as missing data types and viewer engagement metrics are evident. To deepen understanding, incorporating a broader range of data types, expanding variables, and utilizing predictive analytics is recommended. These enhancements will enable Netflix to better tailor content recommendations and stay attuned to evolving viewer preferences.</p>
<div style="text-align: left; padding: 20px; display: flex; align-items: center;">
<div style="flex: 1; margin-right: 20px;">
<div class="container">
  <div class="contact-info">
    <h2>Contact us:</h2>
    <div class="github-link">
      <a href="https://github.com/optimizationworld" target="_blank">
        <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/git%20hub%20logo.png?raw=true" alt="GitHub Logo" style="width: 30px; height: 30px; margin-right: 2px;">
      </a>
      <span>optimizationworld</span>
    </div>
    <div class="github-link">
      <a href="https://www.instagram.com/your_instagram_username" target="_blank">
        <a href="https://www.instagram.com/your_instagram_username" target="_blank">
          <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/phone%20logo.jpg?raw=true" alt="phone Logo" style="width: 30px; height: 30px; margin-right: 2px;">
      </a>
      <span>+971522878400</span>
  </div>
  <div class="github-link>
    <a href="https://www.instagram.com/optimizationworld" target="_blank">
  <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/instagram%20logo%202.png?raw=true" alt="Instagram Logo" style="width: 30px; height: 30px; margin-right: 2px;">
</a>
<span>@optimizationworld </span>
</div>
<div class="github-link>
<a href="https://www.instagram.com/your_instagram_username" target="_blank">
<img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/mail%20logo3.png?raw=true" alt="mail Logo" style="width: 30px; height: 30px; margin-right: 2px;">
</a>
<span>optimizewordly@gmail.com </span>
</div>
  </div>
  <div class="company-logo">
    <img src="https://github.com/optimizationworld/Reports-Data-sciences/blob/main/WO%20logo.png?raw=true" alt="Company Logo" style="width: 300px; height: 300px;">
  </div>
</div>
</div>
</div>
    
</body>
</html>
