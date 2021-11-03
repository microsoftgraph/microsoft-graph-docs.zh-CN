---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04a4d6c7c3e1a922447f881cc420ab9cd20cc3bf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696345"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthoredNote *authoredNote = [[MSGraphAuthoredNote alloc] init];
MSGraphItemBody *content = [[MSGraphItemBody alloc] init];
[content setContent:@"String"];
[content setContentType: [MSGraphBodyType text]];
[authoredNote setContent:content];

NSError *error;
NSData *authoredNoteData = [authoredNote getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authoredNoteData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```