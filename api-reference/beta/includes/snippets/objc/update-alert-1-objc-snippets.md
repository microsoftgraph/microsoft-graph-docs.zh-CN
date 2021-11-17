---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f6cbdeb00f2572082c66d3c3afb0f4a434b61a3093787f866576dc2437f31e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215737"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/alerts/{alert_id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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