---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 204add9a02533d9e2d38ad282d46d2fb8ce76cace62b790bc7e0b7d998352090
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215732"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/alerts/updateAlerts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *valueList = [[NSMutableArray alloc] init];
MSGraphAlert *value = [[MSGraphAlert alloc] init];
[value setAssignedTo:@"String"];
[value setClosedDateTime:@"String (timestamp)"];
NSMutableArray *commentsList = [[NSMutableArray alloc] init];
[commentsList addObject: @"String"];
[value setComments:commentsList];
MSGraphAlertFeedback *feedback = [[MSGraphAlertFeedback alloc] init];
[value setFeedback:feedback];
[value setId:@"String (identifier)"];
MSGraphAlertStatus *status = [[MSGraphAlertStatus alloc] init];
[value setStatus:status];
NSMutableArray *tagsList = [[NSMutableArray alloc] init];
[tagsList addObject: @"String"];
[value setTags:tagsList];
MSGraphSecurityVendorInformation *vendorInformation = [[MSGraphSecurityVendorInformation alloc] init];
[vendorInformation setProvider:@"String"];
[vendorInformation setVendor:@"String"];
[value setVendorInformation:vendorInformation];
[valueList addObject: value];
payloadDictionary[@"value"] = valueList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```