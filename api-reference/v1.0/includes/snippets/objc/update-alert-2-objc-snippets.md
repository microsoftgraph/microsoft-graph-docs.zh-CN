---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 697c106b499898a513539acb810e4bddb45a1fd0549a30e8bfee5d8c5d100814
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162617"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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