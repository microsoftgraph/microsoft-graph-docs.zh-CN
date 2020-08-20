---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88ddae83e05cfa22823c519428d71a28c9d2e1e2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821355"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/anniversaries"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnniversary *personAnniversary = [[MSGraphPersonAnniversary alloc] init];
[personAnniversary setType: [MSGraphAnniversaryType birthday]];
[personAnniversary setDate:@"1980-01-08"];

NSError *error;
NSData *personAnniversaryData = [personAnniversary getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnniversaryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```