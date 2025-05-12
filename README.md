# API Documentation

## Table of Contents
1. [My Courses](#my-courses)
   - 1.1 [Get Paginated Courses](#1-get-paginated-courses)
   - 1.2 [Get Course Module](#2-get-course-module)
   - 1.3 [Get To-Do List](#3-get-to-do-list)
   - 1.4 [Get My Courses](#20-get-my-courses)

2. [Leaderboard](#leaderboard)
   - 2.1 [Get User Rankings](#4-get-user-rankings)
   - 2.2 [Get Category Rankings](#5-get-category-rankings)

3. [Explore](#explore)
   - 3.1 [Get All Categories](#6-get-all-categories)
   - 3.2 [Get Subcategories](#7-get-subcategories)
   - 3.3 [Get Category Courses](#8-get-category-courses)

4. [Knowledge Library](#knowledge-library)
   - 4.1 [Get News Updates](#9-get-news-updates)
   - 4.2 [Get Quiz Corner](#11-get-quiz-corner)
   - 4.3 [Get Survey Corner](#12-get-survey-corner)
   - 4.4 [Get Polls Corner](#14-get-polls-corner)

5. [Media Library](#media-library)
   - 5.1 [Get Media Albums](#10-get-media-library)

6. [Central Library](#central-library)
   - 6.1 [Get Book Categories](#17-get-central-book-library-categories)

7. [Publication Library](#publication-library)
   - 7.1 [Get Publications by Folder](#15-get-publications-by-folder)
   - 7.2 [Get Social File](#16-get-social-file)
   - 7.3 [Get Policy Document](#19-get-policy-document)
8. [Catalog](#catalog)
   - 8.1 [Get My Courses](#81-get-my-courses)
   - 8.2 [Get Course Count](#82-get-course-count)
   - 8.3 [Get Selected Languages](#83-get-selected-languages)
   - 8.4 [Get Course Enrollment Config](#84-get-course-enrollment-config)
   - 8.5 [Get All Categories](#85-get-all-categories)
9. [Competency](#competency)
    - 9.1 [Get Competency Hub Data](#91-get-competency-hub-data)
    - 9.2 [Get Competency Spider Chart](#92-get-competency-spider-chart)
      
10. [Calendar](#calendar)
    - 10.1 [Get Date Format](#101-get-date-format)
    - 10.2 [Get ILT Calendar Data](#102-get-ilt-calendar-data)
    - 10.3 [Check Batch Nomination Status](#103-check-batch-nomination-status)
    - 10.4 [Get Calendar Help Info](#104-get-calendar-help-info)
    - 10.5 [Get Academy List](#105-get-academy-list)
    - 10.6 [Get Organization Calendar](#106-get-organization-calendar)
    - 10.7 [Export ILT Calendar](#107-export-ilt-calendar)
    - 10.8 [Export Trainer Calendar](#108-export-trainer-calendar)
    - 10.9 [Get Schedule Data](#109-get-schedule-data)
    - 10.10 [Get Schedule Count](#1010-get-schedule-count)
    - 10.11 [Check Past Schedule Cancellation](#1011-check-past-schedule-cancellation)
    - 10.12 [Get Localization Strings](#1012-get-localization-strings)
    - 10.13 [Get Nomination Data](#1013-get-nomination-data)
    - 10.14 [Get Nomination Count](#1014-get-nomination-count)
    - 10.15 [Get Training Attendance](#1015-get-training-attendance)
      
11. [Profile](#profile)
    - 11.1 [Get Encrypted User ID](#111-get-encrypted-user-id)
    - 11.2 [Get Profile Permissions](#112-get-profile-permissions)
    - 11.3 [Get User Configurable Parameters](#113-get-user-configurable-parameters)
    - 11.4 [Check Federation ID Status](#114-check-federation-id-status)
    - 11.5 [Get User Profile](#115-get-user-profile)
    - 11.6 [Get User Settings](#116-get-user-settings)
    - 11.7 [Get Profile Picture](#117-get-profile-picture)
    - 11.8 [Get User Details by ID](#118-get-user-details-by-id)
    - 11.9 [Get Competency Status Report](#119-get-competency-status-report)
    - 11.10 [Get Key Area Settings Count](#1110-get-key-area-settings-count)
    - 11.11 [Get Key Area Settings](#1111-get-key-area-settings)
    - 11.12 [Check External Certificate Status](#1112-check-external-certificate-status)
    - 11.13 [Get User Certificates](#1113-get-user-certificates)
    - 11.14 [Get User Certificates Count](#1114-get-user-certificates-count)
    - 11.15 [Check VIMEO Status](#1115-check-vimeo-status)
12. [Course Management](#course-management)
    - 12.1 [Get LCMS Media](#121-get-lcms-media)
    - 12.2 [Get File Format Size](#122-get-file-format-size)
    - 12.3 [Get Media Count](#123-get-media-count)
    - 12.4 [Upload SCORM Content](#124-upload-scorm-content)
    - 12.5 [Upload PDF Content](#125-upload-pdf-content)
13. [Module Management](#module-management)
    - 13.1 [Get Module Data](#131-get-module-data)
    - 13.2 [Get Media Count](#132-get-media-count)
    - 13.3 [Search LCMS Media](#133-search-lcms-media)

## My Courses

### 1. Get Paginated Courses
- **Endpoint**: `GET /api/v1/mycourses/{pageNumber}/{pageSize}/`
- **URL**: `https://gogetempowered.com/api/v1/mycourses/{pageNumber}/{pageSize}/`
- **Authentication**: Bearer Token
- **Parameters**:
  - `pageNumber`: Integer (1-based index)
  - `pageSize`: Integer (items per page)
- **Response**: Array of course objects
```json
[
  {
    "courseId": 28686,
    "title": "Courseassignment1",
    "mission": null,
    "description": "",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb96.jpg",
    "categoryName": "",
    "subCategoryName": null,
    "subSubCategoryName": null,
    "code": "10790",
    "courseFee": 0.0,
    "currency": "",
    "courseType": "elearning",
    "completionPeriodDays": -1,
    "courseCreationdDays": 3,
    "numberofModules": 1,
    "categoryId": null,
    "subCategoryId": null,
    "subSubCategoryId": null,
    "courseRating": 0.0,
    "status": "completed",
    "isFeedback": false,
    "isAssignment": false,
    "isAssessment": false,
    "isPreAssessment": false,
    "isCertificateIssued": false,
    "courseStartDate": "2025-05-04T12:53:05",
    "courseCompleteDate": "2025-05-07T12:53:05",
    "createdDate": null,
    "assignDate": null,
    "rewardPoint": null,
    "isCourseApplicable": true,
    "courseApprovalStatus": "Enrolled",
    "competencyCategory": null,
    "competencyCategoryID": 0,
    "assessmentPercentage": "--",
    "scheduleRequestStatus": "",
    "durationInMinutes": 0,
    "assessmentResult": "--",
    "isPreRequisiteCourse": false,
    "isExternalProvider": false,
    "externalProvider": null,
    "courseURL": null,
    "isRetraining": false,
    "nodalApprovalStatus": "Not Requested",
    "isSCORM": false,
    "firstAccessDate": null,
    "lastAccessDate": null,
    "timeSpent": null,
    "views": 0,
    "progressinpercentage": 0,
    "score": 0,
    "assignmentType": "",
    "courseDueDate": "NA",
    "pathLink": null,
    "alreadyEnrolled": null,
    "totalRating": null,
    "externalDescription": null
  }
]
```

### 2. Get Course Module
- **Endpoint**: `GET /api/v1/mycourses/Getmodule/{courseId}`
- **URL**: `https://go-getempowered.com/api/v1/mycourses/Getmodule/{courseId}`
- **Authentication**: Bearer Token
- **Response**: Detailed course module information
```json
{
  "courseId": 14883,
  "courseType": "elearning",
  "courseCode": "6144",
  "categoryName": "",
  "courseTitle": "new deployment testing",
  "numberofModules": 1,
  "completionPeriodDays": -1,
  "courseFee": 0.0,
  "currency": "",
  "thumbnailPath": "/assets/img/Thumbnail_vectors/img_thumb86.jpg",
  "description": "",
  "learningApproach": false,
  "language": "",
  "courseCreditPoints": 0.0,
  "preAssessmentId": 0,
  "assessmentId": 0,
  "feedbackId": 0,
  "isFeedbackOptional": false,
  "assignmentId": 0,
  "isPreAssessment": false,
  "isAssessment": false,
  "isFeedback": false,
  "isAssignment": false,
  "isCertificateIssued": false,
  "status": "completed",
  "assessmentStatus": "incompleted",
  "preAssessmentStatus": "",
  "feedbackStatus": null,
  "contentStatus": "completed",
  "adminName": "LMS Admin",
  "courseRating": 0.0,
  "courseRatingCount": 0,
  "isAdaptiveLearning": false,
  "progressPercentage": 100,
  "duration": 0,
  "courseAssignedDate": "5/9/2025 12:43:48 PM",
  "lastActivityDate": "3/29/2024 10:36:44 AM",
  "isDilinkingILT": false,
  "assignmentStatus": "",
  "isModuleHasAssFeed": true,
  "isManagerEvaluation": false,
  "managerEvaluationStatus": "NA",
  "isPreRequisiteCourse": false,
  "modules": [
    {
      "moduleId": 14180,
      "moduleName": "External link",
      "mimeType": "",
      "isSecuredContent": false,
      "path": "t5aPAKTyAwf3Nw6CcugNrHZWnaJcijMdzqR7yGFkF+nlB6FaPgG2hwvN6DTeeMFEiuARHoIe3QDLf2e+Np6DcfjtGqDyh8wC1fnf6YIoFWhdzDi10ZXBzmlfSUACMYhH9/CERJNbbiBVXovLk9zuxlkgkNFdDMxTaWhFaxd9DytE7PKSp2eruaUzbI/t3U/B5KjAWzuQYAuIOAhnUOMEmKtgGY5Er4/qiqtIsRYIcB2FmNwQUHtuhR8xrSh14yt7lVDAQInSyLyuW+0KAmvBD26VtlKaOntgSSQ/y6PD2wA=",
      "zipPath": "",
      "moduleType": "externalLink",
      "actualModuleType": null,
      "thumbnail": "",
      "description": "External link",
      "assesmentType": null,
      "isLearnerFeedback": false,
      "isTrainerFeedback": false,
      "isMobileCompatible": true,
      "duration": 0.0,
      "creditPoints": 0,
      "preAssessmentId": 0,
      "assessmentId": 0,
      "feedbackId": 0,
      "lcmsId": 11867,
      "youtubeVideoId": "",
      "externalLCMSId": null,
      "isPreAssessment": false,
      "isAssessment": false,
      "isFeedback": false,
      "status": "completed",
      "assessmentStatus": null,
      "preAssessmentStatus": null,
      "feedbackStatus": null,
      "contentStatus": "completed",
      "sectionId": null,
      "batchId": 0,
      "batchCode": "",
      "batchName": "",
      "scheduleID": 0,
      "scheduleCode": "",
      "startDate": null,
      "endDate": null,
      "registrationEndDate": null,
      "startTime": null,
      "endTime": null,
      "placeName": "",
      "city": "",
      "address": "",
      "trainingRequestStatus": "",
      "sequenceNo": 2,
      "location": "",
      "finalDate": "",
      "completionPeriodDays": 0,
      "isEnableModule": true,
      "activityID": null,
      "isMultilingual": false,
      "selectedLanguageCode": "en",
      "isEmbed": true,
      "bbBmeetingDetails": [],
      "apizooms": null,
      "apiteams": null,
      "apigsuit": null,
      "attendanceStatus": "",
      "waiverStatus": "ATTENDANCE",
      "scheduleCreatedBy": 0,
      "tz_StartDt": "0001-01-01T00:00:00",
      "tz_EndDt": "0001-01-01T00:00:00",
      "academyAgencyName": "",
      "feedbackRating": null,
      "trainerName": null,
      "scheduleFeedbackId": null,
      "scheduleFeedbackStatus": null,
      "assignmentId": 0,
      "isAssignment": false,
      "assignmentStatus": ""
    }
  ],
  "isShowViewBatches": false,
  "expiryMessage": null,
  "isCourseExpired": null,
  "externalProvider": null,
  "externalProviderCategory": null,
  "isOJT": false,
  "ojtStatus": "NA",
  "ojtId": 0,
  "isVisibleAssessmentDetails": true,
  "startDate": "",
  "endDate": "",
  "retrainingDate": "NA",
  "assignmentType": "",
  "feedbackRating": null,
  "aasectId": 0,
  "isANCC": false,
  "faqPath": ""
}
```


### 3. Get To-Do List
- **Endpoint**: `GET /api/v1/ToDoPriorityList/GetToDoList`
- **URL**: `https://gogetempowered.com/api/v1/ToDoPriorityList/GetToDoList`
- **Authentication**: Bearer Token
- **Response**: Array of to-do items
```json
[
  {
    "id": 14,
    "title": "Critical Thinking",
    "scheduleDate": "06 Jan 2025",
    "endDate": "30 Nov 2025",
    "priority": true,
    "status": "completed",
    "type": "Course",
    "moduleType": "MultiModule",
    "assignmentType": ""
  }
]
```

---

## Leaderboard

### 4. Get User Rankings
- **Endpoint**: `POST /api/v1/User/GetRanking`
- **URL**: `https://gogetempowered.com/api/v1/User/GetRanking`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"ranks":10,"configuredColumnName":"undefined","houseCode":null}
```json
{
  "topRanking": [
    {
      "userId": 0,
      "euSerId": "fk2zuGnuQ/lJ2By+PLvNTg==",
      "userName": "LMS Admin",
      "totalPoint": 29952,
      "profilePicture": "enth/638818232516312348.png",
      "gender": "Male",
      "rank": 1,
      "level": "Grand Master",
      "maximumLevelPoint": 1000,
      "levelCode": "LEVEL5",
      "houseCode": "GREEN",
      "houseName": "Green House",
      "eId": "1hYJXXhSkF5gojB+LP0NgA==",
      "country": null,
      "createdDate": "2025-05-09T14:58:43"
    }
  ]
}
```

### 5. Get Category Rankings
- **Endpoint**: `POST /api/v1/User/GetCategoryRanking`
- **URL**: `https://gogetempowered.com/api/v1/User/GetCategoryRanking`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"ranks":10,"configuredColumnName":"","houseCode":null,"configuredColumnValue":""}
  ```
- **Response**: Array of ranked users by category
 ```json
{
  "topRanking": [
    {
      "userId": 0,
      "euSerId": "YHSkA+oXyG5awnev610Vsw==",
      "userName": "Narendra Shete",
      "totalPoint": 20,
      "profilePicture": "",
      "gender": "",
      "rank": 1,
      "level": "Knight 2",
      "maximumLevelPoint": 50,
      "levelCode": "LEVEL1",
      "houseCode": "YELLOW",
      "houseName": "Yellow House",
      "eId": "zuyN1moDThcHeUtBaFEhDA==",
      "country": null,
      "createdDate": "2024-07-17T16:48:55"
    }
  ]
}
```

---

## Explore

### 6. Get All Categories
- **Endpoint**: `GET /api/v1/Category/-1/-1/`
- **URL**: `https://gogetempowered.com/api/v1/Category/-1/-1/`
- **Authentication**: Bearer Token
- **Response**: Array of categories
```json
[
    {
        "id": 179,
        "code": "526",
        "name": "Comprehensive Career Programs",
        "imagePath": "enth/thumbnail/course/638575840919183387.png",
        "sequenceNo": 1
    }
]
```

### 7. Get Subcategories
- **Endpoint**: `GET /api/v1/SubCategory/-1/-1/null/{categoryId}/`
- **URL**: `https://gogetempowered.com/api/v1/SubCategory/-1/-1/null/{categoryId}/`
- **Authentication**: Bearer Token
- **Response**: Array of subcategories
```json
[
    {
        "id": 425,
        "categoryId": 178,
        "code": "SITWD",
        "name": "Product training",
        "categoryName": "Software,IT and Web Development ",
        "sequenceNo": 1,
        "thumbnailPath": null
    }
]
```

### 8. Get Category Courses
- **Endpoint**: `GET /api/v1/mycourses/{page}/{pagesize}/{categoryId}/null/null/null/null/true/true/recently/null/All/null/null/null/null`
- **URL**: `https://gogetempowered.com/api/v1/mycourses/{page}/{pagesize}/{categoryId}/null/null/null/null/true/true/recently/null/All/null/null/null/null`
- **Authentication**: Bearer Token
- **Response**: Array of courses in category
 ```json
[
    {
        "courseId": 16447,
        "title": "gamefication_normal",
        "mission": null,
        "description": "<p>learn about LMS</p>",
        "thumbnailPath": "/assets/img/Thumbnail_vectors/img_thumb26.jpg",
        "categoryName": "Software, IT and Web Development",
        "subCategoryName": "Product training",
        "subSubCategoryName": "LMS training",
        "code": "7026",
        "courseFee": 0.0,
        "currency": "",
        "courseType": "elearning",
        "completionPeriodDays": 3,
        "courseCreationdDays": 0,
        "numberofModules": 2,
        "categoryId": 178,
        "subCategoryId": 425,
        "subSubCategoryId": null,
        "courseRating": 0.0,
        "status": null,
        "isFeedback": false,
        "isAssignment": false,
        "isAssessment": false,
        "isPreAssessment": false,
        "isCertificateIssued": true,
        "courseStartDate": null,
        "courseCompleteDate": null,
        "rewardPoint": null,
        "isCourseApplicable": false,
        "courseApprovalStatus": "",
        "competencyCategory": "--",
        "competencyCategoryID": 0,
        "assessmentPercentage": null,
        "scheduleRequestStatus": "",
        "durationInMinutes": 0,
        "assessmentResult": null,
        "isPreRequisiteCourse": false,
        "isExternalProvider": false,
        "externalProvider": null,
        "courseURL": "",
        "isRetraining": false,
        "nodalApprovalStatus": "Not Requested",
        "isSCORM": false,
        "firstAccessDate": null,
        "lastAccessDate": null,
        "timeSpent": null,
        "views": 0,
        "progressinpercentage": 0,
        "score": 0,
        "assignmentType": "",
        "courseDueDate": "NA",
        "alreadyEnrolled": null,
        "certificationStatus": null
    }
]
```

---

## Knowledge Library

### 9. Get News Updates
- **Endpoint**: `GET /api/v1/NewsUpdates`
- **URL**: `https://gogetempowered.com/api/v1/NewsUpdates`
- **Authentication**: Bearer Token

### 10. Get Media Library
- **Endpoint**: `POST /api/v1/MediaLibrary/AlbumsV2`
- **URL**: `https://gogetempowered.com/api/v1/MediaLibrary/AlbumsV2`
- **Authentication**: Bearer Token
- **Payload**: 
  ```json
  {"page":-1,"pageSize":-1,"search":""}
  ```
- **Response**: Array of media albums
  ```json
  {
    "records": [
      {
        "id": 93,
        "albumName": "test video file"
      }
    ]
  }
  ```
  ### 11. Get Quize Corner
- **Endpoint**: `GET api/v1/QuizzesManagement/GetAllQuizzesManagementForEndUser`
- **URL**: `https://gogetempowered.com/api/v1/QuizzesManagement/GetAllQuizzesManagementForEndUser`
- **Authentication**: Bearer Token
- **Response**: 
```json
[
  {
    "id": 1082,
    "date": "0001-01-01T00:00:00",
    "quizTitle": "Test 2022 Quiz ",
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "targetResponseCount": 0,
    "status": false
  },
  {
    "id": 1090,
    "date": "0001-01-01T00:00:00",
    "quizTitle": "demo 12345",
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "targetResponseCount": 0,
    "status": false
  }
]
```

### 12. Get Survey Corner

- **Endpoint**: `GET /api/v1/SurveyManagement/GetAllSurveyManagementForEndUser`
- **URL**: `https://gogetempowered.com`
- **Authentication**: Bearer Token required

### 13. Get News Updates

- **Endpoint**: `GET /api/v1/NewsUpdates`
- **URL**: `https://gogetempowered.com/api/v1/PollsManagement/GetAllPollsManagementForEndUser`
- **Authentication**: Bearer Token

### 14. Get Polls Corner
- * **Endpoint**: `GET /api/v1/PollsManagement/GetAllPollsManagementForEndUser`
-  **URL**: `https://gogetempowered.com/api/v1/PollsManagement/GetAllPollsManagementForEndUser`
- **Authentication**: Bearer Token

### 15. Get Publications by Folder

- **Endpoint**: `GET /api/v1/Publications/GetAllPublicationsByFolders/{folderId}`
- **URL**: `https://gogetempowered.com/api/v1/Publications/GetAllPublicationsByFolders/null`
- **Authentication**: Bearer Token 
---
### 16. Get Social File

* **Endpoint**: `POST /api/v1/Publications/GetSocialFile`
* **URL**: `https://gogetempowered.com/api/v1/Publications/GetSocialFile`
* **Authentication**: Bearer Token required
* **Request Body** (JSON):

  ```json
  {
    "socialfile": "/enth/Publication/.pdf/638779104850058669.pdf"
  }
  ```
* **Description**:
  Retrieves the specified social PDF file (typically for viewing or downloading).

  
### 17. Get Central Book Library Categories

- **Endpoint**: `GET /api/v1/CentralBookLibrary/GetAllCategory`
- **URL**: `https://gogetempowered.com/api/v1/CentralBookLibrary/GetAllCategory`
- **Authentication**: Bearer Token required

- **Response**: 
```json
[
  {
    "id": 1,
    "category": "Product Management"
  },
  {
    "id": 2,
    "category": "Communication"
  }
]
```
### 18. Get Configurable Parameter Value – SHOW\_POLICYLABEL

- **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/SHOW_POLICYLABEL`
- **URL**: `https://gogetempowered.com/api/v1/ConfigurableParameters/GetValue/SHOW_POLICYLABEL`
- **Authentication**: Bearer Token required

- **Response**: 

```json
{
  "value": "Yes"
}
```


### 19. Get Policy Document

- **Endpoint**: `GET /api/v1/PolicyDocument`
- **URL**: `https://gogetempowered.com/api/v1/PolicyDocument`
- **Authentication**: Bearer Token required

```json
[
  {
    "customerCode": null,
    "applicabilityParameter": null,
    "applicabilityParameterValue": null,
    "applicabilityParameterValueId": null,
    "id": 4,
    "policyId": "enth4",
    "policyDescription": "Quality",
    "commanToAllUser": true,
    "modifiedDate": "11/10/2022 7:05:33 AM",
    "reviewFrequency": "Monthly",
    "ruleId": "Quality4",
    "conditionRegardToOtherRules": "",
    "contentPath": "/enth/.pdf/638036805198254935..pdf",
    "policyLabel": "policy d"
  }
]
```
### 20. Get My Courses 
* **Endpoint**:  
  `GET /api/v1/mycourses/{page}/{pageSize}/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/1/10/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "courseId": 13014,
    "title": "2004",
    "description": "<p>anfjs fdmngjrf dngtltrif sndjf wjsdinc vbfhudsd ndflkj</p>",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb150.jpg",
    "courseType": "elearning",
    "categoryName": "--",
    "courseFee": 0.0,
    "numberofModules": 1,
    "courseRating": 0.0,
    "isCertificateIssued": true,
    "progressinpercentage": 0,
    "score": 0,
    "courseDueDate": "NA",
    "isSCORM": true,
    "nodalApprovalStatus": "Not Requested"
  }
]
```
## Catalog

### 8.1 Get My Courses
* **Endpoint**:  
  `GET /api/v1/mycourses/{page}/{pageSize}/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/1/10/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token
* **Response**:
```json
[
  {
    "courseId": 13014,
    "title": "2004",
    "mission": null,
    "description": "<p>anfjs fdmngjrf dngtltrif sndjf wjsdinc vbfhudsd ndflkj</p>",
    "thumbnailPath": "../../../assets/img/Thumbnail_vectors/img_thumb150.jpg",
    "categoryName": "--",
    "subCategoryName": "",
    "subSubCategoryName": "",
    "code": "5004",
    "courseFee": 0.0,
    "currency": "",
    "courseType": "elearning",
    "completionPeriodDays": 0,
    "courseCreationdDays": 0,
    "numberofModules": 1,
    "categoryId": null,
    "subCategoryId": 0,
    "subSubCategoryId": null,
    "courseRating": 0.0,
    "status": null,
    "isFeedback": false,
    "isAssignment": false,
    "isAssessment": false,
    "isPreAssessment": false,
    "isCertificateIssued": true,
    "isSCORM": true,
    "progressinpercentage": 0,
    "score": 0,
    "courseDueDate": "NA",
    "nodalApprovalStatus": "Not Requested"
  }
]
```

### 8.2 Get Course Count
* **Endpoint**:  
  `GET /api/v1/mycourses/count/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **URL**:  
  `https://gogetempowered.com/api/v1/mycourses/count/null/null/null/null/null/null/true/a-z/null/All/null/null/null/null`

* **Authentication**: Bearer Token

* **Response**:  
  `1284` (Total course count as integer)

### 8.3 Get Selected Languages
* **Endpoint**:  
  `GET /api/v1/Customer/GetSelectedLanguages`

* **URL**:  
  `https://gogetempowered.com/api/v1/Customer/GetSelectedLanguages`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "code": "en",
    "isDeleted": false,
    "name": "English"
  },
  {
    "code": "ar",
    "isDeleted": false,
    "name": "Arabic"
  }
]
```

### 8.4 Get Course Enrollment Config
* **Endpoint**:  
  `GET /api/v1/ConfigurableParameters/GetValue/COURSE_ENROLL`

* **URL**:  
  `https://gogetempowered.com/api/v1/ConfigurableParameters/GetValue/COURSE_ENROLL`

* **Authentication**: Bearer Token

* **Response**:
```json
{
  "value": "TrainingRequest"
}
```

### 8.5 Get All Categories 
* **Endpoint**:  
  `GET /api/v1/Category`

* **URL**:  
  `https://gogetempowered.com/api/v1/Category`

* **Authentication**: Bearer Token

* **Response**:
```json
[
  {
    "id": 179,
    "code": "526",
    "name": "Comprehensive Career Programs",
    "imagePath": "enth/thumbnail/course/638575840919183387.png",
    "sequenceNo": 1
  },
  {
    "id": 178,
    "code": "079",
    "name": "Software,IT and Web Development",
    "imagePath": "enth/thumbnail/course/638575389614925644.png",
    "sequenceNo": 2
  }
]
```


## Competency 

### 9.1 Get Competency Hub Data 
* **Endpoint**: `POST /api/v1/Report/Competency/GetCompetencyHubData`
* **URL**: `https://gogetempowered.com/api/v1/Report/Competency/GetCompetencyHubData`
* **Authentication**: Bearer Token
* **Payload**:
```json
{"Page":1,"PageSize":10}
```
* **Response(Trimed responce)**:
```json
{
  "success": true,
  "data": {
    "records": [
      {
        "categoryName": "negotiation skills",
        "competencyName": "bargaining",
        "competencyID": "288",
        "requiredLevel": "Level 1"
      },
      {
        "categoryName": "Recruiter",
        "competencyName": "Channel",
        "competencyID": "314",
        "requiredLevel": "Level 1"
      }
    ]
  }
}
```

### 9.2 Get Competency Spider Chart 
* **Endpoint**: `GET /api/v1/CompetencyCategory/GetCompetencySpiderchart`
* **URL**: `https://gogetempowered.com/api/v1/CompetencyCategory/GetCompetencySpiderchart`
* **Authentication**: Bearer Token
* **Response(Trimed responce)**:
```json
{
  "counts": [66.67, 50.0, 100.0],
  "competencyName": [
    "Collaboration",
    "Excellence Orientation",
    "Customer Focus"
  ]
}
```

## Calendar

### 10.1 Get Date Format 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/APPLICATION_DATE_FORMAT`
* **Response**: 
```json
{"value":"dd MMM yyyy"}
```

### 10.2 Get ILT Calendar Data 
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderData`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```

### 10.3 Check Batch Nomination Status
* **Endpoint**: `GET /api/v1/c/ILTBatch/IsBatchwiseNominationEnabled`
* **Response**: `"No"`

### 10.4 Get Calendar Help Info
* **Endpoint**: `GET /api/v1/QuickHelpInfo/GetHelpByType/l_cal`

### 10.5 Get Academy List
* **Endpoint**: `GET /api/v1/ILTSchedule/GetAcademyTypeAhead/Internal`
* **Response**:
```json
[
  {"id":1,"title":"MIT"},
  {"id":2,"title":"Enthralltech"}
]
```

### 10.6 Get Organization Calendar
* **Endpoint**: `POST /api/v1/calendar/OrganizationCalenderData`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```
* **Response**:
```json
[
  {
    "courseId": 9734,
    "moduleName": "3742_VILT Type Course",
    "moduleType": "vilt"
  }
]
```

### 10.7 Export ILT Calendar
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderDataExport`
* **Payload**:
```json
{"fromDate":"2025-05-01T00:00:00.000Z","toDate":"2025-06-29T18:30:00.000Z"}
```

### 10.8 Export Trainer Calendar
* **Endpoint**: `POST /api/v1/calendar/ILTCalenderDataForTrainerExport`
* **Payload**: Same as 10.7

### 10.9 Get Schedule Data
* **Endpoint**: `POST /api/v1/ILTSchedule/GetScheduleData`
* **Payload**:
```json
{"Page":1,"PageSize":10,"showAllData":"false"}
```
* **Response**:
```json
[
  {
    "id": 7020,
    "startDate": "2025-05-12T00:00:00",
    "startTime": "15:50:00"
  }
]
```

### 10.10 Get Schedule Count
* **Endpoint**: `GET /api/v1/ILTSchedule/count/null/null/false`
* **Response**: `753`

### 10.11 Check Past Schedule Cancellation
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/Enable_PastScheduleCancel`
* **Response**: 
```json
{"value":"Yes"}
```

### 10.12 Get Localization Strings
* **Endpoint**: `GET /assets/i18n/en.json`
* **Response**:
```json
{
  "SUBMIT_ASSIGNMENT": "Please submit assignment...",
  "CUSTOMER": {
    "HEADER": "Customer Master"
  }
}
```

### 10.13 Get Nomination Data
* **Endpoint**: `POST /api/v1/TrainingNomination/GetNominationData`
* **Payload**:
```json
{"page":1,"pageSize":10,"showAllData":"false"}
```
* **Response**:
```json
[
  {
    "id": 7019,
    "startDate": "2025-05-05T00:00:00"
  }
]
```

### 10.14 Get Nomination Count
* **Endpoint**: `GET /api/v1/TrainingNomination/count/null/null/false`
* **Response**: `622`

### 10.15 Get Training Attendance
* **Endpoint**: `GET /api/v1/ILTTrainingAttendance/1/10/null/null/false`
* **Response**:
```json
[
  {
    "scheduleCode": "SC12745",
    "startDate": "2025-05-12T00:00:00"
  }
]
```

## Profile

### 11.1 Get Encrypted User ID {#111-get-encrypted-user-id}
* **Endpoint**: `POST /api/v1/User/GetEncryptedUserId`
* **Payload**: `{}`
* **Response**:
```json
{"encryptedUserId":"fk2zuGnuQ/lJ2By+PLvNTg=="}
```

### 11.2 Get Profile Permissions

* **Endpoint**: `GET /api/v1/user/GetProfilePermission`
* **Response**:
```json
[
  {
    "name": "Change Password",
    "code": "ch_pass",
    "isAccess": true
  }
]
```

### 11.3 Get User Configurable Parameters
* **Endpoint**: `POST /api/v1/user/UserConfigurableParameter`
* **Payload**:
```json
["HRBP_Rename","Mentor_Rename"]
```
* **Response**:
```json
[
  {
    "code": "HRBP_Rename",
    "value": "HRBP"
  }
]
```

### 11.4 Check Federation ID Status 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/Enable_FederationID`
* **Response**: 
```json
{"value":"No"}
```

### 11.5 Get User Profile
* **Endpoint**: `GET /api/v1/user/GetUserProfile`
* **Response**:
```json
{
  "userName": "LMS Admin",
  "timeZone": "(UTC+05:30) Chennai...",
  "profilePicture": ""
}
```

### 11.6 Get User Settings
* **Endpoint**: `GET /api/v1/user/UserSetting/1/25`
* **Response**:
```json
[
  {
    "configuredColumnName": "Business",
    "fieldType": "TYPEAHEAD"
  }
]
```

### 11.7 Get Profile Picture 
* **Endpoint**: `POST /api/v1/User/GetProfilePicture`
* **Payload**: `{"id":""}`

### 11.8 Get User Details by ID 
* **Endpoint**: `POST /api/v1/User/GetUserDetailsById`
* **Payload**:
```json
{"id":"fk2zuGnuQ/lJ2By+PLvNTg=="}
```
* **Response**:
```json
{
  "userName": "LMS Admin",
  "profilePicture": "enth/638818232516312348.png"
}
```

### 11.9 Get Competency Status Report
* **Endpoint**: `POST /api/v1/Report/Competency/CompetencyStatusReport/Self`
* **Payload**:
```json
{"Page":1,"PageSize":10}
```
* **Response**:
```json
{
  "competencyCharts": [
    {
      "competencyName": "Collaboration",
      "status": "Pending"
    }
  ]
}
```

### 11.10 Get Key Area Settings Count 
* **Endpoint**: `GET /api/v1/KeyAreaSetting/GetMyKeyAreaSettingCount/`
* **Response**: `0`

### 11.11 Get Key Area Settings
* **Endpoint**: `GET /api/v1/KeyAreaSetting/GetMyKeyAreaSetting/1/10/`
* **Response**: `[]`

### 11.12 Check External Certificate Status 
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/ExternalCertificate`
* **Response**: 
```json
{"value":"Yes"}
```

### 11.13 Get User Certificates
* **Endpoint**: `GET /api/v1/CourseCertificateAssociation/GetUserCertificatesByUserId/1/10/null/null`
* **Response**:
```json
[
  {
    "id": 4,
    "category": null
  }
]
```

### 11.14 Get User Certificates Count
* **Endpoint**: `GET /api/v1/CourseCertificateAssociation/GetUserCertificatesByUserIdCount/null/null`
* **Response**: `4`

### 11.15 Check VIMEO Status
* **Endpoint**: `GET /api/v1/ConfigurableParameters/GetValue/VIMEO`
* **Response**: 
```json
{"value":"No"}
```

## Course Management {#course-management}


### 12.1 Get LCMS Media 
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 18,
  "search": "scorm",
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "path": "/assets/courses/638826713822767440Day1_About_Max_12May_NOQus_2004/index_lms.html",
      "contentType": "SCORM1.2",
      "isMobileCompatible": true
    }
  ]
}
```

### 12.2 Get File Format Size
* **Endpoint**: `GET /api/v1/MasterPageSetting/GetFileFormatSize/ADDITIONAL_RESOURCE`
* **Response**:
```json
{
  "id": 28,
  "name": "ADDITIONAL_RESOURCE",
  "size": 51200
}
```

### 12.3 Get Media Count
* **Endpoint**: `GET /api/v1/LCMS/GetMediaCount/true`
* **Response**: Returns integer count of media items


### 12.4 Upload SCORM Content
* **Endpoint**: `POST /api/v1/LCMS`
* **Authentication**: Bearer Token
* **Content-Type**: `multipart/form-data`
* **Required Parameters**:

| Field | Type | Description | Example |
|-------|------|-------------|---------|
| `name` | string | Course name | "History of Agra" |
| `description` | string | Course description | "Journey of Agra to become a National Heritage site" |
| `contentType` | string | MIME type of content | "application/x-zip-compressed" |
| `version` | string | Content version | "1.0" |
| `metaData` | string | Additional metadata | "Indian Historical place" |
| `language` | string | Language code | "en" |
| `scormType` | string | SCORM version | "SCORM1.2" |
| `duration` | integer | Duration in minutes | 60 |
| `isMobileCompatible` | boolean | Mobile compatibility | true |
| `fileForUpload` | binary | ZIP file containing SCORM package | test.zip |

* **Optional Parameters**:
  - `youtubeVideoId`: (string) YouTube video ID if applicable
  - `isBuiltInAssessment`: (boolean) Default false
  - `isSecuredContent`: (boolean) Default false

* **Success Response**: 1

### 12.5 Upload PDF Content
* **Endpoint**: `POST /api/v1/LCMS`
* **Authentication**: Bearer Token required
* **Content-Type**: `multipart/form-data`
* **Request Parameters**:

| Field | Type | Required | Description | Example |
|-------|------|----------|-------------|---------|
| `name` | string | Yes | Content title | "sahich" |
| `description` | string | Yes | Content description | "How sahich became top hotel industry" |
| `contentType` | string | Yes | Must be "application/pdf" | "application/pdf" |
| `version` | string | Yes | Content version | "1.0" |
| `originalFileName` | string | Yes | Original PDF filename | "Document.pdf" |
| `language` | string | Yes | 2-letter language code | "en" |
| `duration` | integer | Yes | Duration in minutes | 60 |
| `fileForUpload` | binary | Yes | PDF file content | - |



## Module Management

### 13.1 Get Module Data
* **Endpoint**: `POST /api/v1/module/GetModuleData`
* **Authentication**: Bearer Token
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 10,
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 18498,
      "name": "sahich",
      "moduleType": "Document",
      "description": "sahich",
      "isActive": true,
      "createdBy": 2549,
      "userName": "LMS Admin"
    }
  ]
}
```

### 13.2 Get Media Count
* **Endpoint**: `GET /api/v1/LCMS/GetMediaCount/true`
* **Authentication**: Bearer Token
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "contentType": "SCORM1.2",
      "isMobileCompatible": true,
      "duration": 60.0
    }
  ]
}
```

### 13.3 Search LCMS Media
* **Endpoint**: `POST /api/v1/LCMS/GetLCMSMedia`
* **Authentication**: Bearer Token
* **Payload**:
```json
{
  "page": 1,
  "pageSize": 12,
  "search": "scorm",
  "showAllData": "false"
}
```
* **Response**:
```json
{
  "data": [
    {
      "id": 16004,
      "name": "Day 1_About_Max_12May_NOQus_2004",
      "path": "/assets/courses/.../index_lms.html",
      "contentType": "SCORM1.2",
      "duration": 60.0,
      "language": "en"
    }
  ]
}
```




### Implementation Notes:
1. All endpoints require Bearer Token authentication
2. Category/Subcategory endpoints use -1 for unlimited results


