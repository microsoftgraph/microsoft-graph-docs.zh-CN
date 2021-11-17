---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54ab63220c141b0744fd98944558c4ae980368632fd748827290436177170df7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279492"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/anniversaries"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnnualEvent *personAnnualEvent = [[MSGraphPersonAnnualEvent alloc] init];
[personAnnualEvent setType: [MSGraphPersonAnnualEventType birthday]];
[personAnnualEvent setDate:@"1980-01-08"];

NSError *error;
NSData *personAnnualEventData = [personAnnualEvent getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnnualEventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```