---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47ebf900d1cfdb2e38aecff581df7f0b9270c5a3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996581"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/anniversaries"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnniversary *personAnniversary = [[MSGraphPersonAnniversary alloc] init];
[personAnniversary setType: [MSGraphAnniversaryType birthday]];
[personAnniversary setDate:@"datetime-value"];

NSError *error;
NSData *personAnniversaryData = [personAnniversary getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnniversaryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```