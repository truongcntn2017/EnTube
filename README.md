# EnTube: A dataset for Youtube video engagement analytics

YouTube, one of the largest online video-sharing platforms today, has provided a place for content creators to share information and earn extra income. Anticipating whether a video will be engaged by viewers or not is an essential factor in helping video creators improve video content and quality before publishing. To facilitate this task, we build an annotated dataset of 23,738 videos collected from 72 YouTube channels in Vietnam that were in four categories (i.e., comedy, travel-and-events, education, science-and-technology) and published over 12 years. We evaluate a number of metrics for measuring video engagement to propose a novel measure which determines the engagement of a video via its: Q score. Using our proposed measure, we annotate videos with three levels of engagement including: Engage, Neutral, and not Engage. From the supervised dataset, we constructed a multimodal to infer the degree of engagement based on  the content of a YouTube video such as title, audio, thumbnail, video, and tags. We believe our dataset and metric to be useful for engagement analytic as well as studies on social media content.

# Table of Contents
1. [Meta data](#Metadata)
2. [Missing rate](#MissingRate)
3. [Sample data](#Data)

## Metadata


| Column     | Description  |
| -------    | -----------  |
| channel\_id                               | Id of channel             |
|    channel\_name                               | Name of channel                   |
|        channel\_category                         | Category of channel                  |
|        channel\_started                              | Started year of channel                   |
|        channel\_rank                               | Rank of channel in most-subscribed Vietnamese channels |
|        channel\_subscribers                             | Number of subscribers of channel          |
|       id                             | Id of video         |
|        title                             | Title of video          |
|        length\_title                             | Length title of video (tokens)         |
|        categories                             | Categories of video        |
|        description                             | Description of video        |
|        tags                             | Tags of video        |
|        num\_tags                             | Number of tags of video        |
|        upload\_date                             | Uploaded date of video        |
|        delta\_upload\_date                             | Distance between collected date and uploaded date (days) |
|        duration                             | Duration of video (minutes)     |
|        view\_count                             | Number of views of video     |
|        like\_count                             | Number of likes of video     |
|        comment\_count                             | Number of comments of video     |
|        dislike\_count                             | Number of dislikes of video     |
|        like\_per\_view                             | Number of likes per views of video     |
|        comment\_per\_view                             | Number of comments per views of video     |
|        dislike\_per\_view                             | Number of dislikes per views of video     |
|        engagement\_rate\_1                             | Total comments and likes per views of video     |
|        engagement\_rate\_2                            | Total comments, likes, and dislikes per views of video    |
|        q\_score                           | Q score of video    |
|        label\_1                           | Engagement level based on engagement\_rate\_1 of video    |
|        label\_2                           | Engagement level based on q\_score of video     |

## Missing Rate


| Column     | Description  |
| -------    | -----------  |
| channel\_id                               | 0.000000           |
|    channel\_name                               | 0.000000                |
|        channel\_category                         | 0.000000                 |
|        channel\_started                              | 0.000000                |
|        channel\_rank                               | 0.000000 |
|        channel\_subscribers                             | 0.000000         |
|       id                             | 0.000000    |
|        title                             | 0.000000      |
|        length\_title                             | 0.000000    |
|        categories                             | 0.000000     |
|        description                             | 0.017609        |
|        tags                             | 0.000000     |
|        num\_tags                             | 0.000000      |
|        upload\_date                             | 0.000000   |
|        delta\_upload\_date                             | 0.000000 |
|        duration                             | 0.000000     |
|        view\_count                             | 0.000000    |
|        like\_count                             | 0.000000   |
|        comment\_count                             | 0.000000    |
|        dislike\_count                             | 0.000000    |
|        like\_per\_view                             | 0.000000  |
|        comment\_per\_view                             | 0.000000    |
|        dislike\_per\_view                             | 0.000000    |
|        engagement\_rate\_1                             | 0.000000     |
|        engagement\_rate\_2                            | 0.000000    |
|        q\_score                           | 0.000000   |
|        label\_1                           | 0.000000    |
|        label\_2                           | 0.000000   |


## Data

* sample/audio_by_year: folder contains audio by year
* sample/thumbnails_by_year: folder contains thumbnails by year
* sample/video_by_year: folder contains video by year
* sample/entube_final.parquet: files contains metadata
