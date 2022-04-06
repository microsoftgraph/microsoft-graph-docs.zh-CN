---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a21bad82533bba99b86fb8a88c95efe1b5bcffa9
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528101"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBaseTask *baseTask = [[MSGraphBaseTask alloc] init];
[baseTask setTextBody:@"String"];
[baseTask setBodyLastModifiedDateTime:@"String (timestamp)"];
[baseTask setCompletedDateTime:@"String (timestamp)"];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[baseTask setDueDateTime:dueDateTime];
MSGraphDateTimeTimeZone *startDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[baseTask setStartDateTime:startDateTime];
[baseTask setImportance: [MSGraphImportance low]];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
[baseTask setRecurrence:recurrence];
[baseTask setDisplayName:@"String"];
[baseTask setStatus: [MSGraphTaskStatus_v2 notStarted]];
MSGraphTaskViewpoint *viewpoint = [[MSGraphTaskViewpoint alloc] init];
[baseTask setViewpoint:viewpoint];

NSError *error;
NSData *baseTaskData = [baseTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:baseTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```