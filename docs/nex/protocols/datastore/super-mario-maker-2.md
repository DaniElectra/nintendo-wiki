---
layout: post
toc: true
title: Super Mario Maker 2 (115)
---

This page describes the methods that are only seen in Super Mario Maker 2.

Some methods take a `resultOption` parameter. This parameter controls which fields are looked up in the database. Fields that are not specified in the `resultOption` parameter are usually returned as zero or empty.

## Methods

| Method ID | Method Name                                                                    |
| --------- | ------------------------------------------------------------------------------ |
| 47        | [RegisterUser](#47-registeruser)                                               |
| 48        | [GetUsers](#48-getusers)                                                       |
| 49        | [SyncUserProfile](#49-syncuserprofile)                                         |
| 50        | [SearchUsersUserPoint](#50-searchusersuserpoint)                               |
| 51        | [SearchUsersEndlessMode](#51-searchusersendlessmode)                           |
| 52        | [SearchUsersBattleMode](#52-searchusersbattlemode)                             |
| 53        | [SearchUsersPlayedCourse](#53-searchusersplayedcourse)                         |
| 54        | [SearchUsersClearedCourse](#54-searchusersclearedcourse)                       |
| 55        | [SearchUsersPositiveRatedCourse](#55-searchuserspositiveratedcourse)           |
| 56        | [SearchUsersFollowee](#56-searchusersfollowee)                                 |
| 57        | [SearchUsersClearRanking](#57-searchusersclearranking)                         |
| 58        | [SearchUsersTermsRanking](#58-searchuserstermsranking)                         |
| 59        | [UpdateLastLoginTime](#59-updatelastlogintime)                                 |
| 60        | [CanPostCourse](#60-canpostcourse)                                             |
| 61        | [CanPostRatingAndComment](#61-canpostratingandcomment)                         |
| 62        | [UpdateMiiClothes](#62-updatemiiclothes)                                       |
| 63        | [GetMiiClothes](#63-getmiiclothes)                                             |
| 64        | [PostActivityQuest](#64-postactivityquest)                                     |
| 65        | [GetUserNameNgType](#65-getusernamengtype)                                     |
| 66        | [PreparePostObjectCourse](#66-preparepostobjectcourse)                         |
| 67        | CompletePostObjectCourse                                                       |
| 68        | [CompletePostObjectsCourse](#68-completepostobjectscourse)                     |
| 69        | [UpdateCourseTag](#69-updatecoursetag)                                         |
| 70        | [GetCourses](#70-GetCourses)                                                   |
| 71        | [SearchCoursesPointRanking](#71-searchcoursespointranking)                     |
| 72        | [SearchCoursesAdvanced](#72-searchcoursesadvanced)                             |
| 73        | [SearchCoursesLatest](#73-searchcourseslatest)                                 |
| 74        | [SearchCoursesPostedBy](#74-searchcoursespostedby)                             |
| 75        | [SearchCoursesPositiveRatedBy](#75-searchcoursespositiveratedby)               |
| 76        | [SearchCoursesPlayedBy](#76-searchcoursesplayedby)                             |
| 77        | [SearchCoursesBattleMode](#77-searchcoursesbattlemode)                         |
| 78        | [SearchCoursesBattleModeByDifficulty](#78-searchcoursesbattlemodebydifficulty) |
| 79        | [SearchCoursesEndlessMode](#79-searchcoursesendlessmode)                       |
| 80        | [SearchCoursesFirstClear](#80-searchcoursesfirstclear)                         |
| 81        | [SearchCoursesBestTime](#81-searchcoursesbesttime)                             |
| 82        | [SearchCoursesFolloweePostedBy](#82-searchcoursesfolloweepostedby)             |
| 83        | [SearchCoursesTermsRanking](#83-searchcoursestermsranking)                     |
| 84        | [SearchCoursesPickUp](#84-searchcoursespickup)                                 |
| 85        | [GetCoursesEvent](#85-getcoursesevent)                                         |
| 86        | [SearchCoursesEvent](#86-searchcoursesevent)                                   |
| 87        | [ReadEventCourseList](#87-readeventcourselist)                                 |
| 88        | PreparePostObjectCommentPicture                                                |
| 89        | CompletePostObjectCommentPicture                                               |
| 90        | CompletePostObjectsCommentPicture                                              |
| 91        | PostCommentText                                                                |
| 92        | PostCommentStamp                                                               |
| 93        | DeleteComment                                                                  |
| 94        | [SearchCommentsInOrder](#94-searchcommentsinorder)                             |
| 95        | [SearchComments](#95-searchcomments)                                           |
| 96        | PostPlayResult                                                                 |
| 97        | PostPlayResults                                                                |
| 98        | PostPlayResultsAccumulated                                                     |
| 99        | PostPlayResultBattleModePersonal                                               |
| 100       | PostPlayResultBattleModeEntire                                                 |
| 101       | PostPlayResultMultiClear                                                       |
| 102       | PostPlayResultEventCourse                                                      |
| 103       | [GetDeathPositions](#103-getdeathpositions)                                    |
| 104       | [PostRatingInfo](#104-postratinginfo)                                          |
| 105       | PostRatingInfos                                                                |
| 106       | PostRatingInfoBattleModePersonal                                               |
| 107       | PostRatingInfoBattleModeEntire                                                 |
| 108       | [GetEndlessModeStatus](#108-getendlessmodestatus)                              |
| 109       | InitEndlessMode                                                                |
| 110       | StartEndlessModeCourse                                                         |
| 111       | DominateEndlessModeCourse                                                      |
| 112       | PassEndlessModeCourse                                                          |
| 113       | SuspendEndlessMode                                                             |
| 114       | FinishEndlessMode                                                              |
| 115       | GetEndlessModePlayInfo                                                         |
| 116       | GetEndlessModeRank                                                             |
| 117       | [GetBattleModeRating](#117-getbattlemoderating)                                |
| 118       | [StartBattleMode](#118-startbattlemode)                                        |
| 119       | [EndBattleMode](#119-endbattlemode)                                            |
| 120       | ForceEndBattleMode                                                             |
| 121       | StartMultiClear                                                                |
| 122       | EndMultiClear                                                                  |
| 123       | FollowUser                                                                     |
| 124       | UnfollowUser                                                                   |
| 125       | GetNewNotification                                                             |
| 126       | ReadNewNotification                                                            |
| 127       | GetNotification                                                                |
| 128       | ReadNotification                                                               |
| 129       | GetNgCourseNotification                                                        |
| 130       | GetOperatingInformation                                                        |
| 131       | [GetUserOrCourse](#131-getuserorcourse)                                        |
| 132       | [PreparePostRelationObject](#132-preparepostrelationobject)                    |
| 133       | CompletePostRelationObject                                                     |
| 134       | [GetReqGetInfoHeadersInfo](#134-getreqgetinfoheadersinfo)                      |
| 135       | [CanReportFromCourseInfo](#135-canreportfromcourseinfo)                        |
| 136       | [CanReportFromCommentInfo](#136-canreportfromcommentinfo)                      |
| 137       | [CanReportFromUserInfo](#137-canreportfromuserinfo)                            |
| 138       | [CanReportFromBugDetection](#138-canreportfrombugdetection)                    |
| 139       | ReportFromCourseInfo                                                           |
| 140       | ReportFromCommentInfo                                                          |
| 141       | ReportFromUserInfo                                                             |
| 142       | ReportFromBugDetection                                                         |
| 143       | GetAdditionalMiiClothes                                                        |
| 144       | GetAdditionalMiiClothesReqGetInfos                                             |
| 145       | DebugPreparePostObjectAdditionalMiiClothes                                     |
| 146       | DebugCompletePostObjectAdditionalMiiClothes                                    |
| 147       | SearchUsersOfficial                                                            |
| 148       | PostPlayResultCoop                                                             |
| 149       | PostPlayResultBattleModeFriendPersonal                                         |
| 150       | PostPlayResultBattleModeFriendEntire                                           |
| 151       | LoginCheck                                                                     |
| 152       | UpdateLastLoginInfo                                                            |
| 153       | [GetEventCourseStamp](#153-geteventcoursestamp)                                |
| 154       | [GetEventCourseStatus](#154-geteventcoursestatus)                              |
| 155       | [ReadEventCourseResult](#155-readeventcourseghostresult)                       |
| 156       | [GetEventCourseHistogram](#156-geteventcoursehistogram)                        |
| 157       | [GetEventCourseGhost](#157-geteventcourseghost)                                |
| 158       | [DebugUploadEventCourseGhost](#158-debuguploadeventcourseghost)                |
| 159       | [RegisterWorldMap](#159-registerworldmap)                                      |
| 160       | [GetWorldMap](#160-getworldmap)                                                |
| 161       | [SearchWorldMapPlayedBy](#161-searchworldmapplayedby)                          |
| 162       | [SearchWorldMapPickUp](#162-searchworldmappickup)                              |
| 163       | [GetWorldMapProgress](#163-getworldmapprogress)                                |
| 164       | [DeleteWorldMap](#164-deleteworldmap)                                          |
| 165       | [InitializeWorldMapProgress](#165-initializeworldmapprogress)                  |
| 166       | [UpdateWorldMapProgress](#166-updateworldmapprogress)                          |
| 167       | GetUsersFriend                                                                 |
| 168       | SearchUsersFolloweeV2                                                          |
| 169       | GetEventCourseFriendGhost                                                      |

### (47) RegisterUser
#### Request

| Type                                              | Description |
| ------------------------------------------------- | ----------- |
| [RegisterUserParam](#registeruserparam-structure) | Param       |

#### Response
This method does not return anything.

### (48) GetUsers
#### Request

| Type                                      | Description |
| ----------------------------------------- | ----------- |
| [GetUsersParam](#getusersparam-structure) | Param       |

#### Response

| Type                     | Description  |
| ------------------------ | ------------ |
| [List]&lt;[UserInfo]&gt; | Users        |
| [List]&lt;[Result]&gt;   | Result codes |

### (49) SyncUserProfile
#### Request

| Type                                                    | Description |
| ------------------------------------------------------- | ----------- |
| [SyncUserProfileParam](#syncuserprofileparam-structure) | Param       |

#### Response

| Type                                                      | Description |
| --------------------------------------------------------- | ----------- |
| [SyncUserProfileResult](#syncuserprofileresult-structure) | Result      |

### (50) SearchUsersUserPoint
#### Request

| Type                                                              | Description |
| ----------------------------------------------------------------- | ----------- |
| [SearchUsersUserPointParam](#searchusersuserpointparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| [List]&lt;Uint32&gt;     | Ranks       |
| Bool                     | Result      |

### (51) SearchUsersEndlessMode
#### Request

| Type                                                                  | Description |
| --------------------------------------------------------------------- | ----------- |
| [SearchUsersEndlessModeParam](#searchusersendlessmodeparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| [List]&lt;Uint32&gt;     | Unknown     |
| Bool                     | Unknown     |

### (52) SearchUsersBattleMode
#### Request

| Type                                                                | Description |
| ------------------------------------------------------------------- | ----------- |
| [SearchUsersBattleModeParam](#searchusersbattlemodeparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| [List]&lt;Uint32&gt;     | Unknown     |
| Bool                     | Unknown     |

### (53) SearchUsersPlayedCourse
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [SearchUsersPlayedCourseParam](#searchusersplayedcourseparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |

### (54) SearchUsersClearedCourse
#### Request

| Type                                                                      | Description |
| ------------------------------------------------------------------------- | ----------- |
| [SearchUsersClearedCourseParam](#searchusersclearedcourseparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |

### (55) SearchUsersPositiveRatedCourse
#### Request

| Type                                                                             | Description |
| -------------------------------------------------------------------------------- | ----------- |
| [SearchUsersPositiveRatedCourse](#searchuserspositiveratedcourseparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |

### (56) SearchUsersFollowee
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [SearchUsersFolloweeParam](#searchusersfolloweeparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| Bool                     | Unknown     |

### (57) SearchUsersClearRanking
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [SearchUsersClearRankingParam](#searchusersclearrankingparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| [List]&lt;Uint32&gt;     | Unknown     |
| Bool                     | Unknown     |

### (58) SearchUsersTermsRanking
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [SearchUsersTermsRankingParam](#searchuserstermsrankingparam-structure) | Param       |

#### Response

| Type                     | Description |
| ------------------------ | ----------- |
| [List]&lt;[UserInfo]&gt; | Users       |
| [List]&lt;Uint32&gt;     | Unknown     |
| Bool                     | Unknown     |

### (59) UpdateLastLoginTime
#### Request
This method does not take any parameters.

#### Response
This method does not return anything.

### (60) CanPostCourse
#### Request
This method does not take any parameters.

#### Response

| Type   | Description |
| ------ | ----------- |
| Bool   | Unknown     |
| Uint32 | Unknown     |

### (61) CanPostRatingAndComment
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [CanPostRatingAndCommentParam](#canpostratingandcommentparam-structure) | Param       |

#### Response

| Type                                                                      | Description |
| ------------------------------------------------------------------------- | ----------- |
| [CanPostRatingAndCommentResult](#canpostratingandcommentresult-structure) | Result      |

### (62) UpdateMiiClothes
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [List]&lt;[UpdateMiiClothesParam](#updatemiiclothesparam-structure)&gt; | Param       |

#### Response
This method does not return anything.

### (63) GetMiiClothes
#### Request
This method does not take any parameters.

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[MiiClothes]&gt; | Mii clothes |

### (64) PostActivityQuest
#### Request

| Type                 | Description |
| -------------------- | ----------- |
| [List]&lt;Uint32&gt; | Unknown     |

#### Response
This method does not return anything.

### (65) GetUserNameNgType
#### Request
This method does not take any parameters.

#### Response

| Type  | Description |
| ----- | ----------- |
| Uint8 | Type        |

### (66) PreparePostObjectCourse
#### Request

| Type                                                        | Description |
| ----------------------------------------------------------- | ----------- |
| [PreparePostCourseParam](#preparepostcourseparam-structure) | Param       |

#### Response

| Type                   | Description |
| ---------------------- | ----------- |
| [DataStoreReqPostInfo] | Info        |

### (68) CompletePostObjectsCourse
#### Request

| Type                                                                        | Description |
| --------------------------------------------------------------------------- | ----------- |
| [CompletePostObjectsCourseParam](#completepostobjectscourseparam-structure) | Param       |

#### Response
This method does not return anything.

### (69) UpdateCourseTag
#### Request

| Type                                                    | Description |
| ------------------------------------------------------- | ----------- |
| [UpdateCourseTagParam](#updatecoursetagparam-structure) | Param       |

#### Response
This method does not return anything.

### (70) GetCourses
#### Request

| Type                                          | Description |
| --------------------------------------------- | ----------- |
| [GetCoursesParam](#getcoursesparam-structure) | Param       |

#### Response

| Type                       | Description  |
| -------------------------- | ------------ |
| [List]&lt;[CourseInfo]&gt; | Course info  |
| [List]&lt;[Result]&gt;     | Result codes |

### (71) SearchCoursesPointRanking
#### Request

| Type                                                                        | Description |
| --------------------------------------------------------------------------- | ----------- |
| [SearchCoursesPointRankingParam](#searchcoursespointrankingparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Course info |
| [List]&lt;Uint32&gt;       | Ranks       |
| Bool                       | Result      |

### (72) SearchCoursesAdvanced
#### Request

| Type                                                                | Description |
| ------------------------------------------------------------------- | ----------- |
| [SearchCoursesAdvancedParam](#searchcoursesadvancedparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Course info |
| Bool                       | Result      |

### (73) SearchCoursesLatest
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [SearchCoursesLatestParam](#searchcourseslatestparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| Bool                       | Result      |

### (74) SearchCoursesPostedBy
#### Request

| Type                                                                | Description |
| ------------------------------------------------------------------- | ----------- |
| [SearchCoursesPostedByParam](#searchcoursespostedbyparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| Bool                       | Result      |

### (75) SearchCoursesPositiveRatedBy
#### Request

| Type                                                                              | Description |
| --------------------------------------------------------------------------------- | ----------- |
| [SearchCoursesPositiveRatedByParam](#searchcoursespositiveratedbyparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (76) SearchCoursesPlayedBy
#### Request

| Type                                                                          | Description |
| ----------------------------------------------------------------------------- | ----------- |
| [SearchCoursesPlayedByParam](#searchcoursesplayedbyparam-structure-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (77) SearchCoursesBattleMode
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [SearchCoursesBattleModeParam](#searchcoursesbattlemodeparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (78) SearchCoursesBattleModeByDifficulty
#### Request

| Type                                                                                            | Description |
| ----------------------------------------------------------------------------------------------- | ----------- |
| [SearchCoursesBattleModeByDifficultyParam](#searchcoursesbattlemodebydifficultyparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (79) SearchCoursesEndlessMode
#### Request

| Type                                                                      | Description |
| ------------------------------------------------------------------------- | ----------- |
| [SearchCoursesEndlessModeParam](#searchcoursesendlessmodeparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (80) SearchCoursesFirstClear
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [SearchCoursesFirstClearParam](#searchcoursesfirstclearparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| Bool                       | Result      |

### (81) SearchCoursesBestTime
#### Request

| Type                                                                | Description |
| ------------------------------------------------------------------- | ----------- |
| [SearchCoursesBestTimeParam](#searchcoursesbesttimeparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| Bool                       | Result      |

### (82) SearchCoursesFolloweePostedBy
#### Request

| Type                                                                                | Description |
| ----------------------------------------------------------------------------------- | ----------- |
| [SearchCoursesFolloweePostedByParam](#searchcoursesfolloweepostedbyparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| Bool                       | Result      |

### (83) SearchCoursesTermsRanking
#### Request

| Type                                                                        | Description |
| --------------------------------------------------------------------------- | ----------- |
| [SearchCoursesTermsRankingParam](#searchcoursestermsrankingparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |
| [List]&lt;Uint32&gt;       | Ranks       |
| Bool                       | Result      |

### (84) SearchCoursesPickUp
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [SearchCoursesPickUpParam](#searchcoursespickupparam-structure) | Param       |

#### Response

| Type                       | Description |
| -------------------------- | ----------- |
| [List]&lt;[CourseInfo]&gt; | Courses     |

### (85) GetCoursesEvent
#### Request

| Type                                                    | Description  |
| ------------------------------------------------------- | ------------ |
| [GetCoursesParam](#getcoursesparam-structure)           | Course param |
| [GetCoursesEventParam](#getcourseseventparam-structure) | Event param  |

#### Response

| Type                                                        | Description   |
| ----------------------------------------------------------- | ------------- |
| [List]&lt;[EventCourseInfo](#eventcourseinfo-structure)&gt; | Event courses |
| [List]&lt;[Result]&gt;                                      | Results       |

### (86) SearchCoursesEvent
#### Request

| Type                                                          | Description |
| ------------------------------------------------------------- | ----------- |
| [SearchCoursesEventParam](#searchcourseseventparam-structure) | Event param |

#### Response

| Type                                                        | Description   |
| ----------------------------------------------------------- | ------------- |
| [List]&lt;[EventCourseInfo](#eventcourseinfo-structure)&gt; | Event courses |

### (87) ReadEventCourseList
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [ReadEventCourseListParam](#readeventcourselistparam-structure) | Param       |

#### Response
This method does not return anything.

### (94) SearchCommentsInOrder
#### Request

| Type                                                                | Description |
| ------------------------------------------------------------------- | ----------- |
| [SearchCommentsInOrderParam](#searchcommentsinorderparam-structure) | Param       |

#### Response

| Type                        | Description |
| --------------------------- | ----------- |
| [List]&lt;[CommentInfo]&gt; | Comments    |
| Bool                        | Unknown     |

### (95) SearchComments
#### Request

| Type   | Description |
| ------ | ----------- |
| Uint64 | Data id     |

#### Response

| Type                        | Description |
| --------------------------- | ----------- |
| [List]&lt;[CommentInfo]&gt; | Comments    |

### (103) GetDeathPositions
#### Request

| Type   | Description |
| ------ | ----------- |
| Uint64 | Data id     |

#### Response

| Type                              | Description     |
| --------------------------------- | --------------- |
| [List]&lt;[DeathPositionInfo]&gt; | Death positions |

### (104) PostRatingInfo
#### Request

| Type         | Description |
|--------------|-------------|
| [RatingInfo] | Rating info |

#### Response
This method does not return anything.

### (108) GetEndlessModeStatus
#### Request
This method does not take any parameters.

#### Response

| Type                                              | Description |
| ------------------------------------------------- | ----------- |
| [EndlessModeStatus](#endlessmodestatus-structure) | Result      |

### (117) GetBattleModeRating
#### Request
This method does not take any parameters.

#### Response

| Type               | Description |
| ------------------ | ----------- |
| Bool               | Unknown     |
| [BattleModeRating] | Rating 1    |
| [BattleModeRating] | Rating 2    |

### (118) StartBattleMode
#### Request

| Type                                                    | Description |
| ------------------------------------------------------- | ----------- |
| [StartBattleModeParam](#startbattlemodeparam-structure) | Param       |

#### Response
This method does not return anything.

### (119) EndBattleMode
#### Request

| Type                                                | Description |
| --------------------------------------------------- | ----------- |
| [EndBattleModeParam](#endbattlemodeparam-structure) | Param       |

#### Response

| Type               | Description |
| ------------------ | ----------- |
| [BattleModeRating] | Rating 1    |
| [BattleModeRating] | Rating 2    |

### (131) GetUserOrCourse
#### Request

| Type                                                    | Description |
| ------------------------------------------------------- | ----------- |
| [GetUserOrCourseParam](#getuserorcourseparam-structure) | Param       |

#### Response

| Type         | Description |
| ------------ | ----------- |
| [UserInfo]   | User info   |
| [CourseInfo] | Course info |

### (132) PreparePostRelationObject
#### Request

| Type                                                                        | Description |
| --------------------------------------------------------------------------- | ----------- |
| [PreparePostRelationObjectParam](#preparepostrelationobjectparam-structure) | Info        |

#### Response

| Type                                                              | Description |
| ----------------------------------------------------------------- | ----------- |
| [RelationObjectReqPostInfo](#relationobjectreqpostinfo-structure) | Param       |

### (134) GetReqGetInfoHeadersInfo
This method returns headers that can be used to download relation files from the cloudfront datastore server.

#### Request

| Type  | Description                      |
| ----- | -------------------------------- |
| Uint8 | [Data type](#relation-data-type) |

#### Relation Data Type

| Value | Directory                                        |
| ----- | ------------------------------------------------ |
| 2     | /ds/1/relation_data/course_one_screen_thumbnail/ |
| 3     | /ds/1/relation_data/course_entire_thumbnail/     |
| 10    | /ds/1/comment/                                   |
| 40    | /ds/1/relation_data/event_course_ghost/          |

#### Response

| Type                                                      | Description |
| --------------------------------------------------------- | ----------- |
| [ReqGetInfoHeadersInfo](#reqgetinfoheadersinfo-structure) | Info        |

### (135) CanReportFromCourseInfo
#### Request

| Type   | Description |
| ------ | ----------- |
| Uint64 | Unknown     |

#### Response

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |

### (136) CanReportFromCommentInfo
#### Request

| Type     | Description |
| -------- | ----------- |
| [String] | Unknown     |

#### Response

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |

### (137) CanReportFromUserInfo
#### Request

| Type     | Description |
| -------- | ----------- |
| Uint64   | Unknown     |
| [String] | Unknown     |

#### Response

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |

### (138) CanReportFromBugDetection
#### Request

| Type   | Description |
| ------ | ----------- |
| Uint64 | Unknown     |

#### Response

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |

### (153) GetEventCourseStamp
#### Request
This method does not take any parameters.

#### Response

| Type   | Description |
| ------ | ----------- |
| Uint32 | Stamps      |

### (154) GetEventCourseStatus
#### Request
This method does not take any parameters.

#### Response

| Type                                                      | Description |
| --------------------------------------------------------- | ----------- |
| [EventCourseStatusInfo](#eventcoursestatusinfo-structure) | Status info |

### (155) ReadEventCourseResult
#### Request

| Type   | Description |
| ------ | ----------- |
| Uint64 | Unknown     |

#### Response
This method does not return anything.

### (156) GetEventCourseHistogram
#### Request

| Type                                                                    | Description |
| ----------------------------------------------------------------------- | ----------- |
| [GetEventCourseHistogramParam](#geteventcoursehistogramparam-structure) | Param       |

#### Response

| Type                                                    | Description    |
| ------------------------------------------------------- | -------------- |
| [EventCourseHistogram](#eventcoursehistogram-structure) | Histogram info |

### (157) GetEventCourseGhost
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [GetEventCourseGhostParam](#geteventcourseghostparam-structure) | Param       |

#### Response

| Type                                                                  | Description |
| --------------------------------------------------------------------- | ----------- |
| [List]&lt;[EventCourseGhostInfo](#eventcourseghostinfo-structure)&gt; | Ghosts      |

### (158) DebugUploadEventCourseGhost
#### Request

| Type                                                                            | Description |
| ------------------------------------------------------------------------------- | ----------- |
| [DebugUploadEventCourseGhostParam](#debuguploadeventcourseghostparam-structure) | Param       |

#### Response
This method does not return anything.

### (159) RegisterWorldMap
#### Request

| Type                                                      | Description |
| --------------------------------------------------------- | ----------- |
| [RegisterWorldMapParam](#registerworldmapparam-structure) | Param       |

#### Response
This method does not return anything.

### (160) GetWorldMap
#### Request

| Type                                            | Description |
| ----------------------------------------------- | ----------- |
| [GetWorldMapParam](#getworldmapparam-structure) | Param       |

#### Response

| Type                         | Description |
| ---------------------------- | ----------- |
| [List]&lt;[WorldMapInfo]&gt; | World maps  |
| [List]&lt;[Result]&gt;       | Results     |

### (161) SearchWorldMapPlayedBy
#### Request

| Type                                                                  | Description |
| --------------------------------------------------------------------- | ----------- |
| [SearchWorldMapPlayedByParam](#searchworldmapplayedbyparam-structure) | Param       |

#### Response

| Type                         | Description |
| ---------------------------- | ----------- |
| [List]&lt;[WorldMapInfo]&gt; | World maps  |

### (162) SearchWorldMapPickUp
#### Request

| Type                                                              | Description |
| ----------------------------------------------------------------- | ----------- |
| [SearchWorldMapPickUpParam](#searchworldmappickupparam-structure) | Param       |

#### Response

| Type                         | Description |
| ---------------------------- | ----------- |
| [List]&lt;[WorldMapInfo]&gt; | World maps  |

### (163) GetWorldMapProgress
#### Request

| Type                                                            | Description |
| --------------------------------------------------------------- | ----------- |
| [GetWorldMapProgressParam](#getworldmapprogressparam-structure) | Param       |

#### Response

| Type                                                    | Description   |
| ------------------------------------------------------- | ------------- |
| [WorldMapProgressInfo](#worldmapprogressinfo-structure) | Progress info |

### (164) DeleteWorldMap
#### Request
This method does not take any parameters.

#### Response
This method does not return anything.

### (165) InitializeWorldMapProgress
#### Request

| Type                                                                          | Description |
| ----------------------------------------------------------------------------- | ----------- |
| [InitializeWorldMapProgressParam](#initializeworldmapprogressparam-structure) | Param       |

#### Response
This method does not return anything.

### (166) UpdateWorldMapProgress
#### Request

| Type                                                                  | Description |
| --------------------------------------------------------------------- | ----------- |
| [UpdateWorldMapProgressParam](#updateworldmapprogressparam-structure) | Param       |

#### Response
This method does not return anything.

## Types
### BadgeInfo ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint16 | Unknown     |
| Uint8  | Unknown     |

### BattleModeRating ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |
| Uint8  | Unknown     |

### CanPostRatingAndCommentParam ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint64 | Unknown     |
| Uint32 | Unknown     |

### CanPostRatingAndCommentResult ([Structure])

| Type                       | Description |
| -------------------------- | ----------- |
| Uint64                     | Unknown     |
| Bool                       | Unknown     |
| Uint32                     | Unknown     |
| [Map]&lt;Uint8, Uint32&gt; | Unknown     |
| Bool                       | Unknown     |
| Uint32                     | Unknown     |
| [Map]&lt;Uint8, Uint32&gt; | Unknown     |

### CommentInfo ([Structure])

| Type                                     | Description          |
| ---------------------------------------- | -------------------- |
| Uint64                                   | Unknown              |
| [String]                                 | Unknown              |
| Uint8                                    | Unknown              |
| Uint8                                    | Unknown              |
| Uint64                                   | Unknown              |
| Uint16                                   | Unknown              |
| Uint16                                   | Unknown              |
| Uint8                                    | Unknown              |
| Uint8                                    | Unknown              |
| Uint16                                   | Unknown              |
| Bool                                     | Unknown              |
| Bool                                     | Unknown              |
| [DateTime]                               | Unknown              |
| [qBuffer]                                | Unknown              |
| [String]                                 | Unknown              |
| [CommentPictureReqGetInfoWithoutHeaders] | Comment picture info |
| Uint16                                   | Unknown              |
| Uint8                                    | Unknown              |

### CommentPictureReqGetInfoWithoutHeaders ([Structure])

| Type     | Description        |
| -------- | ------------------ |
| [String] | Url                |
| Uint8    | Relation data type |
| Uint32   | Filesize           |
| [Buffer] | Root ca cert       |
| [String] | Filename           |

### CompletePostObjectsCourseParam ([Structure])

| Type                                                        | Description  |
| ----------------------------------------------------------- | ------------ |
| [String]                                                    | Unknown      |
| [String]                                                    | Unknown      |
| [String]                                                    | Unknown      |
| [String]                                                    | Unknown      |
| [String]                                                    | Unknown      |
| Uint64                                                      | Unknown      |
| [PreparePostCourseParam](#preparepostcourseparam-structure) | Course param |

### CourseInfo ([Structure])

| Type                                          | Option  | Description                         |
| --------------------------------------------- | ------- | ----------------------------------- |
| Uint64                                        |         | Data id                             |
| [String]                                      |         | Level code                          |
| [PID]                                         |         | Owner id                            |
| [String]                                      |         | Level name                          |
| [String]                                      |         | Description                         |
| Uint8                                         |         | [Game style](#game-style)           |
| Uint8                                         |         | [Course theme](#course-theme)       |
| [DateTime]                                    |         | Upload time                         |
| Uint8                                         |         | [Difficulty](#difficulty-level)     |
| Uint8                                         |         | [First tag](#course-tag)            |
| Uint8                                         |         | [Second tag](#course-tag)           |
| Uint8                                         |         | Unknown                             |
| Uint32                                        |         | [Clear condition](#clear-condition) |
| Uint16                                        |         | Clear condition magnitude           |
| Uint16                                        |         | Unknown                             |
| [qBuffer]                                     |         | Unknown                             |
| [Map]&lt;Uint8, Uint32&gt;                    | `0x1`   | [Play stats](#course-play-stats)    |
| [Map]&lt;Uint8, Uint32&gt;                    | `0x2`   | [Course ratings](#course-ratings)   |
| [Map]&lt;Uint8, Uint32&gt;                    | `0x40`  | Unknown                             |
| [CourseTimeStats](#coursetimestats-structure) | `0x4`   | Time stats                          |
| [Map]&lt;Uint8, Uint32&gt;                    | `0x8`   | [Comment stats](#comment-stats)     |
| Uint8                                         | `0x10`  | Unknown                             |
| Uint8                                         | `0x20`  | Unknown                             |
| Uint8                                         | `0x10`  | Unknown                             |
| Uint8                                         | `0x20`  | Unknown                             |
| [RelationObjectReqGetInfo]                    | `0x80`  | One-screen thumbnail                |
| [RelationObjectReqGetInfo]                    | `0x100` | Entire thumbnail                    |

### Game Style

| Value | Description |
| ----- | ----------- |
| 0     | SMB1        |
| 1     | SMB3        |
| 2     | SMW         |
| 3     | NSMBU       |
| 4     | SM3DW       |

### Course Theme

| Value | Description |
| ----- | ----------- |
| 0     | Overworld   |
| 1     | Underground |
| 2     | Castle      |
| 3     | Airship     |
| 4     | Underwater  |
| 5     | Ghost house |
| 6     | Snow        |
| 7     | Desert      |
| 8     | Sky         |
| 9     | Forest      |

### Clear Condition

| Value      | Description      |
| ---------- | ---------------- |
| 0          | None             |
| 4042480826 | Kill skipsqueaks |
| 4116396131 | Collect coins    |

### Course Play Stats

| Key | Description         |
| --- | ------------------- |
| 0   | Plays               |
| 1   | Attempts            |
| 2   | Unknown             |
| 3   | Clears              |
| 4   | Plays (versus mode) |

### Course Ratings

| Key | Description |
| --- | ----------- |
| 0   | Hearts      |
| 1   | Unknown     |
| 2   | Unknown     |

### Comment Stats

| Key | Description        |
| --- | ------------------ |
| 0   | Number of comments |

### CourseTimeStats ([Structure])

| Type   | Description                     |
| ------ | ------------------------------- |
| [PID]  | User id of first completion     |
| [PID]  | User id of world record holder  |
| Uint32 | World record (milliseconds)     |
| Uint32 | Time of uploader (milliseconds) |

### DeathPositionInfo ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint64 | Data id     |
| Uint32 | X           |
| Uint32 | Y           |
| Bool   | Is subworld |

### DebugUploadEventCourseGhostParam ([Structure])

| Type     | Description |
| -------- | ----------- |
| Uint64   | Unknown     |
| Uint32   | Unknown     |
| [String] | Unknown     |

### EndBattleModeParam ([Structure])

| Type                       | Name              |
| -------------------------- | ----------------- |
| [Map]&lt;Uint64, Uint8&gt; | battleResults     |
| Uint32                     | killCount         |
| Uint32                     | killedCount       |
| Uint32                     | glicko2Rate       |
| Uint32                     | glicko2Deviation  |
| Uint32                     | glicko2Volatility |

### EndlessModeStatus ([Structure])

| Type                                 | Description |
| ------------------------------------ | ----------- |
| [Map]&lt;Uint8, [UnknownStruct4]&gt; | Unknown     |
| [Map]&lt;Uint8, [UnknownStruct5]&gt; | Unknown     |

### EventCourseGhostInfo ([Structure])

| Type                       | Description          |
| -------------------------- | -------------------- |
| [RelationObjectReqGetInfo] | Replay file          |
| Uint32                     | Time in milliseconds |
| [PID]                      | User id              |

### EventCourseHistogram ([Structure])

| Type                       | Description                                              |
| -------------------------- | -------------------------------------------------------- |
| Uint64                     | Data id                                                  |
| Uint32                     | Unknown                                                  |
| Uint32                     | Unknown                                                  |
| Uint32                     | Unknown                                                  |
| [List]&lt;Uint32&gt;       | Histogram values                                         |
| [Map]&lt;Uint8, Uint32&gt; | Medal time<br>`50`: Bronze<br>`30`: Silver<br>`10`: Gold |
| Uint32                     | Unknown                                                  |

### EventCourseInfo ([Structure])

| Type                                                    | Option | Description                   |
| ------------------------------------------------------- | ------ | ----------------------------- |
| Uint64                                                  |        | Data id                       |
| [String]                                                |        | Name                          |
| [String]                                                |        | Description                   |
| Uint8                                                   |        | [Game style](#game-style)     |
| Uint8                                                   |        | [Course theme](#course-theme) |
| Bool                                                    | `0x40` | Unknown                       |
| Bool                                                    |        | Unknown                       |
| [DateTime]                                              |        | Upload time                   |
| [DataStoreReqGetInfo]                                   | `0x2`  | GET request info              |
| [Map]&lt;Uint8, Uint32&gt;                              | `0x1`  | Unknown                       |
| [UnknownStruct6](#unknownstruct6-structure)             |        | Unknown                       |
| Uint8                                                   |        | Unknown                       |
| [EventCourseThumbnail](#eventcoursethumbnail-structure) | `0x10` | One-screen thumbnail          |
| [EventCourseThumbnail](#eventcoursethumbnail-structure) | `0x20` | Entire thumbnail              |

Revision 1:

| Type                       | Option  | Description              |
| -------------------------- | ------- | ------------------------ |
| [DateTime]                 |         | Deadline                 |
| Uint8                      |         | Unknown                  |
| Uint32                     |         | Unknown                  |
| Uint16                     |         | Unknown                  |
| Uint16                     |         | Unknown                  |
| Uint32                     | `0x8`   | Personal best time       |
| Uint32                     |         | Unknown                  |
| Uint32                     | `0x100` | Time required for medal  |
| [RelationObjectReqGetInfo] | `0x200` | Personal best time ghost |

### EventCourseStatusInfo ([Structure])

| Type       | Description |
| ---------- | ----------- |
| Uint64     | Unknown     |
| Bool       | Unknown     |
| [DateTime] | Unknown     |

### EventCourseThumbnail ([Structure])

| Type                              | Description  |
| --------------------------------- | ------------ |
| [String]                          | Url          |
| [List]&lt;[DataStoreKeyValue]&gt; | Headers      |
| Uint32                            | Filesize     |
| [Buffer]                          | Root ca cert |
| [String]                          | Filename     |

### GetCoursesParam ([Structure])

| Type                 | Description    |
| -------------------- | -------------- |
| [List]&lt;Uint64&gt; | Data ids       |
| Uint32               | Result options |

## GetCoursesEventParam ([Structure])
This structure is empty.

### GetEventCourseGhostParam ([Structure])

| Type   | Description      |
| ------ | ---------------- |
| Uint64 | Data id          |
| Uint32 | Approximate time |
| Uint8  | Number of ghosts |

### GetEventCourseHistogramParam ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint64 | Data id     |

### GetUserOrCourseParam ([Structure])

| Type     | Name               |
| -------- | ------------------ |
| [String] | codeString         |
| Uint32   | userResultOption   |
| Uint32   | courseResultOption |

### GetUsersParam ([Structure])

| Type                | Name         |
| ------------------- | ------------ |
| [List]&lt;[PID]&gt; | userPIDs     |
| Uint32              | resultOption |

### GetWorldMapParam ([Structure])

| Type                   | Description   |
| ---------------------- | ------------- |
| [List]&lt;[String]&gt; | Ids           |
| Uint32                 | Result option |

### GetWorldMapProgressParam ([Structure])

| Type     | Description |
| -------- | ----------- |
| [String] | Id          |

### InitializeWorldMapProgressParam ([Structure])

| Type     | Description |
| -------- | ----------- |
| [String] | Id          |
| Uint32   | Unknown     |

### MiiClothes ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint16 | Unknown     |
| Uint16 | Unknown     |
| Bool   | Unknown     |

### PreparePostCourseParam ([Structure])

| Type                   | Description |
| ---------------------- | ----------- |
| [String]               | Unknown     |
| [String]               | Unknown     |
| Uint32                 | Unknown     |
| Bool                   | Unknown     |
| Uint8                  | Unknown     |
| Uint8                  | Unknown     |
| Uint32                 | Unknown     |
| Uint32                 | Unknown     |
| Uint32                 | Unknown     |
| Uint32                 | Unknown     |
| [qBuffer]              | Unknown     |
| Uint8                  | Unknown     |
| Uint32                 | Unknown     |
| Uint16                 | Unknown     |
| Uint16                 | Unknown     |
| Bool                   | Unknown     |
| Uint32                 | Unknown     |
| Uint32                 | Unknown     |
| [List]&lt;[String]&gt; | Unknown     |

### PreparePostRelationObjectParam ([Structure])

| Type                   | Name    |
| ---------------------- | ------- |
| [String]               | Unknown |
| Uint32                 | Unknown |
| Uint32                 | Unknown |
| Uint32                 | Unknown |
| Uint32                 | Unknown |
| [List]&lt;[String]&gt; | Unknown |

### RatingInfo ([Structure])

| Type   | Description |
|--------|-------------|
| Uint64 | Unknown     |
| Uint8  | Unknown     |
| Uint8  | Unknown     |
| Bool   | Unknown     |

### ReadEventCourseListParam ([Structure])

| Type       | Description |
| ---------- | ----------- |
| [DateTime] | Unknown     |

### RegisterUserParam ([Structure])

| Type             | Description      |
| ---------------- | ---------------- |
| [String]         | Username         |
| [UnknownStruct1] | Unknown          |
| [qBuffer]        | Unknown          |
| Uint8            | Region id        |
| [String]         | Country code     |
| [String]         | Pseudo device id |

### RegisterWorldMapParam ([Structure])

| Type                 | Description |
| -------------------- | ----------- |
| [qBuffer]            | Unknown     |
| [List]&lt;Uint64&gt; | Unknown     |
| [String]             | Unknown     |
| Uint8                | Unknown     |
| Uint8                | Unknown     |
| Uint32               | Unknown     |

### RelationObjectReqGetInfo ([Structure])

| Type     | Description        |
| -------- | ------------------ |
| [String] | Url                |
| Uint8    | Relation data type |
| Uint32   | Filesize           |
| [Buffer] | Root ca cert       |
| [String] | Filename           |

### RelationObjectReqPostInfo ([Structure])

| Type                              | Description  |
| --------------------------------- | ------------ |
| [String]                          | Data id      |
| [String]                          | Url          |
| [List]&lt;[DataStoreKeyValue]&gt; | Headers      |
| [List]&lt;[DataStoreKeyValue]&gt; | Form fields  |
| [Buffer]                          | Root ca cert |

### ReqGetInfoHeadersInfo ([Structure])

| Type                              | Description          |
| --------------------------------- | -------------------- |
| [List]&lt;[DataStoreKeyValue]&gt; | Headers              |
| Uint32                            | Expiration (seconds) |

### SearchCommentsInOrderParam ([Structure])

| Type          | Name        |
| ------------- | ----------- |
| Uint64        | dataId      |
| [ResultRange] | resultRange |

### SearchCoursesAdvancedParam ([Structure])

| Type                | Name                   |
| ------------------- | ---------------------- |
| Uint32              | resultOption           |
| [ResultRange]       | resultRange            |
| Uint8               | preferCourseDifficulty |
| Uint8               | preferGameSkinId       |
| Uint8               | preferSceneSetId       |
| [List]&lt;Uint8&gt; | preferTagIds           |
| [List]&lt;Uint8&gt; | rejectRegionIds        |
| Uint8               | sortType               |

### SearchCoursesBattleModeParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint32 | resultOption |
| Uint32 | count        |

### SearchCoursesBattleModeByDifficultyParam ([Structure])

| Type   | Description   |
| ------ | ------------- |
| Uint32 | Result option |
| Uint32 | Count         |
| Uint8  | Difficulty    |

### SearchCoursesBestTimeParam ([Structure])

| Type          | Name         |
| ------------- | ------------ |
| [PID]         | pid          |
| Uint32        | resultOption |
| [ResultRange] | resultRange  |

### SearchCoursesEndlessModeParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint32 | resultOption |
| Uint32 | count        |
| Uint8  | difficulty   |

### SearchCoursesEventParam ([Structure])

| Type   | Description   |
| ------ | ------------- |
| Uint32 | Result option |

### SearchCoursesFirstClearParam ([Structure])

| Type          | Description  |
| ------------- | ------------ |
| Uint64        | Unknown      |
| Uint32        | Unknown      |
| [ResultRange] | Result range |

### SearchCoursesFolloweePostedByParam ([Structure])

| Type          | Name         |
| ------------- | ------------ |
| Uint32        | resultOption |
| [ResultRange] | resultRange  |

### SearchCoursesLatestParam ([Structure])

| Type          | Name         |
| ------------- | ------------ |
| Uint32        | resultOption |
| [ResultRange] | resultRange  |

### SearchCoursesPickUpParam ([Structure])

| Type   | Description               |
| ------ | ------------------------- |
| Uint32 | Unknown                   |
| Uint32 | Unknown                   |
| Uint8  | [Difficulty](#difficulty) |

### SearchCoursesPlayedByParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint32 | resultOption |
| Uint32 | count        |
| [PID]  | playerPID    |

### SearchCoursesPointRankingParam ([Structure])

| Type                | Name                   |
| ------------------- | ---------------------- |
| Uint32              | resultOption           |
| [ResultRange]       | resultRange            |
| Uint8               | preferCourseDifficulty |
| [List]&lt;Uint8&gt; | rejectRegionIds        |

### SearchCoursesPositiveRatedByParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint32 | resultOption |
| Uint32 | count        |
| [PID]  | raterPID     |

### SearchCoursesPostedByParam ([Structure])

| Type                | Name         |
| ------------------- | ------------ |
| Uint32              | resultOption |
| [ResultRange]       | resultRange  |
| [List]&lt;[PID]&gt; | ownerPIDs    |

### SearchCoursesTermsRankingParam ([Structure])

| Type          | Description |
| ------------- | ----------- |
| Uint32        | Unknown     |
| [ResultRange] | Unknown     |
| Uint8         | Unknown     |
| [Buffer]      | Unknown     |

### SearchUsersBattleModeParam ([Structure])

| Type          | Description |
| ------------- | ----------- |
| Uint32        | Unknown     |
| [Buffer]      | Unknown     |
| [ResultRange] | Unknown     |

### SearchUsersClearedCourseParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint64 | dataId       |
| Uint32 | resultOption |
| Uint32 | count        |

### SearchUsersClearRankingParam ([Structure])

| Type          | Description |
| ------------- | ----------- |
| Uint8         | Unknown     |
| Uint32        | Unknown     |
| [Buffer]      | Unknown     |
| [ResultRange] | Unknown     |

### SearchUsersEndlessModeParam ([Structure])

| Type          | Description |
| ------------- | ----------- |
| Uint8         | Unknown     |
| Uint32        | Unknown     |
| [Buffer]      | Unknown     |
| [ResultRange] | Unknown     |

### SearchUsersFolloweeParam ([Structure])

| Type          | Name         |
| ------------- | ------------ |
| Uint32        | resultOption |
| [ResultRange] | resultRange  |

### SearchUsersPlayedCourseParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint64 | dataId       |
| Uint32 | resultOption |
| Uint32 | count        |

### SearchUsersPositiveRatedCourseParam ([Structure])

| Type   | Name         |
| ------ | ------------ |
| Uint64 | dataId       |
| Uint32 | resultOption |
| Uint32 | count        |

### SearchUsersUserPointParam ([Structure])

| Type          | Description   |
| ------------- | ------------- |
| Uint32        | Result option |
| [Buffer]      | Unknown       |
| [ResultRange] | Result range  |

### SearchUsersTermsRankingParam ([Structure])

| Type          | Description   |
| ------------- | ------------- |
| Uint32        | Result option |
| [ResultRange] | Result range  |
| [Buffer]      | Unknown       |

### SearchWorldMapPickUpParam ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |

### SearchWorldMapPlayedByParam ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint32 | Unknown     |
| Uint32 | Unknown     |

### UpdateWorldMapProgressParam ([Structure])

| Type      | Description |
| --------- | ----------- |
| [String]  | Id          |
| Uint64    | Unknown     |
| Uint64    | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint32    | Unknown     |
| Uint32    | Unknown     |
| [qBuffer] | Unknown     |

### StartBattleModeParam ([Structure])

| Type                | Name   |
| ------------------- | ------ |
| Uint64              | dataId |
| Uint32              | gid    |
| [List]&lt;[PID]&gt; | pids   |

### SyncUserProfileParam ([Structure])

| Type             | Description      |
| ---------------- | ---------------- |
| [String]         | Username         |
| [UnknownStruct1] | Unknown          |
| [qBuffer]        | Unknown          |
| Uint8            | Unknown          |
| [String]         | Country code     |
| Bool             | Unknown          |
| Bool             | Unknown          |
| [String]         | Pseudo device id |
| Uint32           | Unknown          |

### SyncUserProfileResult ([Structure])

| Type             | Description  |
| ---------------- | ------------ |
| [PID]            | User id      |
| [String]         | Username     |
| [UnknownStruct1] | Unknown      |
| [qBuffer]        | Unknown      |
| Uint8            | Unknown      |
| [String]         | Country code |
| Uint8            | Unknown      |
| Bool             | Unknown      |
| Bool             | Unknown      |

### UnknownStruct1 ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint16 | Unknown     |
| Uint16 | Unknown     |
| Uint16 | Unknown     |
| Uint16 | Unknown     |

### UnknownStruct3 ([Structure])

| Type       | Description |
| ---------- | ----------- |
| Uint8      | Unknown     |
| [DateTime] | Unknown     |

### UnknownStruct4 ([Structure])

| Type       | Description |
| ---------- | ----------- |
| Uint8      | Unknown     |
| Uint8      | Unknown     |
| Uint32     | Unknown     |
| [DateTime] | Unknown     |
| [DateTime] | Unknown     |
| Uint8      | Unknown     |
| Uint8      | Unknown     |

### UnknownStruct5 ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint8  | Unknown     |
| Uint32 | Unknown     |

### UnknownStruct6 ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint64 | Unknown     |
| Uint32 | Unknown     |

### UpdateCourseTagParam ([Structure])

| Type   | Name                  |
| ------ | --------------------- |
| Uint64 | dataId                |
| Uint8  | [tagId1](#course-tag) |
| Uint8  | [tagId2](#course-tag) |

### UpdateMiiClothesParam ([Structure])

| Type   | Description |
| ------ | ----------- |
| Uint16 | Unknown     |
| Uint16 | Unknown     |
| Bool   | Unknown     |

### UserInfo ([Structure])

| Type                       | Option  | Description                                  |
| -------------------------- | ------- | -------------------------------------------- |
| [PID]                      |         | User id                                      |
| [String]                   |         | Maker code                                   |
| [String]                   |         | User name                                    |
| [UnknownStruct1]           | `0x200` | Unknown                                      |
| [qBuffer]                  | `0x4`   | Unknown                                      |
| [String]                   |         | Country code                                 |
| Uint8                      |         | Region id                                    |
| [DateTime]                 |         | Last active time                             |
| Bool                       |         | Unknown                                      |
| Bool                       |         | Unknown                                      |
| Bool                       |         | Unknown                                      |
| [Map]&lt;Uint8, Uint32&gt; | `0x1`   | [Play stats](#user-play-stats)               |
| [Map]&lt;Uint8, Uint32&gt; | `0x2`   | [Maker stats](#maker-stats)                  |
| [Map]&lt;Uint8, Uint32&gt; | `0x8`   | [Endless mode highscores](#difficulty-level) |
| [Map]&lt;Uint8, Uint32&gt; | `0x10`  | [Multiplayer stats](#multiplayer-stats)      |
| [Map]&lt;Uint8, Uint32&gt; | `0x400` | Unknown                                      |
| [List]&lt;[BadgeInfo]&gt;  | `0x20`  | Badge info                                   |
| [Map]&lt;Uint8, Uint32&gt; | `0x40`  | Unknown                                      |
| [Map]&lt;Uint8, Uint32&gt; | `0x80`  | Unknown                                      |

Revision 1:

| Type       | Option   | Description |
| ---------- | -------- | ----------- |
| Bool       |          | Unknown     |
| [DateTime] | `0x1000` | Unknown     |
| Bool       |          | Unknown     |

Revision 2:

| Type             | Option   | Description |
| ---------------- | -------- | ----------- |
| [UnknownStruct3] | `0x2000` | Unknown     |

Revision 3:

| Type                       | Option   | Description |
| -------------------------- | -------- | ----------- |
| [String]                   |          | Unknown     |
| [Map]&lt;Uint8, Uint32&gt; | `0x8000` | Unknown     |
| Bool                       |          | Unknown     |

### User Play Stats

| Key | Description |
| --- | ----------- |
| 0   | Plays       |
| 1   | Clears      |
| 2   | Attempts    |
| 3   | Deaths      |

### Maker Stats

| Key | Description     |
| --- | --------------- |
| 0   | Hearts received |
| 1   | Maker points    |

### Multiplayer Stats

| Key | Description       |
| --- | ----------------- |
| 0   | Multiplayer score |
| 2   | Versus plays      |
| 3   | Versus wins       |
| 10  | Coop plays        |
| 11  | Coop wins         |

### WorldMapInfo ([Structure])

| Type                       | Description |
| -------------------------- | ----------- |
| [String]                   | Id          |
| [PID]                      | Owner pid   |
| [qBuffer]                  | Unknown     |
| [RelationObjectReqGetInfo] | Thumbnail   |
| Uint8                      | Worlds      |
| Uint8                      | Levels      |
| Uint8                      | Unknown     |
| [DateTime]                 | Unknown     |
| [List]&lt;Uint64&gt;       | Data ids    |
| [Map]&lt;Uint8, Uint32&gt; | Unknown     |
| Uint32                     | Unknown     |
| Uint8                      | Unknown     |
| Uint8                      | Unknown     |

### WorldMapProgressInfo ([Structure])

| Type      | Description |
| --------- | ----------- |
| Uint8     | Unknown     |
| [String]  | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint32    | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint8     | Unknown     |
| Uint64    | Unknown     |
| Uint64    | Unknown     |
| [qBuffer] | Unknown     |
| Uint32    | Unknown     |

## Enums
### Course Tag

| Value | Description        |
| ----- | ------------------ |
| 0     | None               |
| 1     | Standard           |
| 2     | Puzzle solving     |
| 3     | Speedrun           |
| 4     | Autoscroll         |
| 5     | Auto mario         |
| 6     | Short and sweet    |
| 7     | Multiplayer versus |
| 8     | Themed             |
| 9     | Music              |
| 10    | Art                |
| 11    | Technical          |
| 12    | Shooter            |
| 13    | Boss battle        |
| 14    | Single player      |
| 15    | Link               |

### Difficulty Level

| Value | Description  |
| ----- | ------------ |
| 0     | Easy         |
| 1     | Normal       |
| 2     | Expert       |
| 3     | Super expert |
| 4     | Any          |


[UnknownStruct1]: #unknownstruct1-structure
[UnknownStruct2]: #unknownstruct2-structure
[UnknownStruct3]: #unknownstruct3-structure
[UnknownStruct4]: #unknownstruct4-structure
[UnknownStruct5]: #unknownstruct5-structure

[UserInfo]: #userinfo-structure
[CourseInfo]: #courseinfo-structure
[BadgeInfo]: #badgeinfo-structure
[RelationObjectReqGetInfo]: #relationobjectreqgetinfo-structure
[CommentInfo]: #commentinfo-structure
[CommentPictureReqGetInfoWithoutHeaders]: #commentpicturereqgetinfowithoutheaders-structure
[MiiClothes]: #miiclothes-structure
[BattleModeRating]: #battlemoderating-structure
[DeathPositionInfo]: #deathpositioninfo-structure
[WorldMapInfo]: #worldmapinfo-structure
[RatingInfo]: #ratinginfo-structure

[DataStoreGetMetaParam]: /docs/nex/protocols/datastore#datastoregetmetaparam-structure
[DataStorePreparePostParam]: /docs/nex/protocols/datastore#datastorepreparepostparam-structure
[DataStoreCompletePostParam]: /docs/nex/protocols/datastore#datastorecompletepostparam-structure
[DataStoreReqGetInfo]: /docs/nex/protocols/datastore#datastorereqgetinfo-structure
[DataStoreReqPostInfo]: /docs/nex/protocols/datastore#datastorereqpostinfo-structure
[DataStoreMetaInfo]: /docs/nex/protocols/datastore#datastoremetainfo-structure
[DataStoreKeyValue]: /docs/nex/protocols/datastore#datastorekeyvalue-structure

[Result]: /docs/nex/types#result
[String]: /docs/nex/types#string
[Buffer]: /docs/nex/types#buffer
[qBuffer]: /docs/nex/types#qbuffer
[List]: /docs/nex/types#list
[Map]: /docs/nex/types#map
[DateTime]: /docs/nex/types#datetime
[Structure]: /docs/nex/types#structure
[Data]: /docs/nex/types#anydataholder
[PID]: /docs/nex/types#pid
[ResultRange]: /docs/nex/types#resultrange-structure
