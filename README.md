# API Documentation

## Table of Contents
1. [My Courses](#my-courses)
2. [Leaderboard](#leaderboard)
3. [Explore](#explore)
4. [Knowledge Library](#knowledge-library)

---

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


---

### Implementation Notes:
1. All endpoints require Bearer Token authentication
2. Category/Subcategory endpoints use -1 for unlimited results


