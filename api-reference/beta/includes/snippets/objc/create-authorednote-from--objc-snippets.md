---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04d81a1f13cdfb8a2450443fe16d51171543cfca
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561813"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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