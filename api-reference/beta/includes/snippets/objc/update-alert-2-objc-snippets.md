---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5cf2c1c34d0ecb412c9c17a8b4bd4ae371b17f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942803"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/alerts/{alert_id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAlert *alert = [[MSGraphAlert alloc] init];
[alert setAssignedTo:@"String"];
[alert setClosedDateTime:@"String (timestamp)"];
NSMutableArray *commentsList = [[NSMutableArray alloc] init];
[commentsList addObject: @"String"];
[alert setComments:commentsList];
[alert setFeedback: [MSGraphAlertFeedback unknown]];
[alert setStatus: [MSGraphAlertStatus unknown]];
NSMutableArray *tagsList = [[NSMutableArray alloc] init];
[tagsList addObject: @"String"];
[alert setTags:tagsList];
MSGraphSecurityVendorInformation *vendorInformation = [[MSGraphSecurityVendorInformation alloc] init];
[vendorInformation setProvider:@"String"];
[vendorInformation setVendor:@"String"];
[alert setVendorInformation:vendorInformation];

NSError *error;
NSData *alertData = [alert getSerializedDataWithError:&error];
[urlRequest setHTTPBody:alertData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```