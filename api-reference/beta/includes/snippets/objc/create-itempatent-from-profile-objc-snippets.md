---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3c7bed492a51b6fe65546646d268d8f22a1c093
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820283"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/patents"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPatent *itemPatent = [[MSGraphItemPatent alloc] init];
[itemPatent setDescription:@"Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel."];
[itemPatent setDisplayName:@"Inferring User Intent through browsing behaviors"];
[itemPatent setIsPending: true];
[itemPatent setNumber:@"USPTO-3954432633"];
[itemPatent setWebUrl:@"https://patents.gov/3954432633"];

NSError *error;
NSData *itemPatentData = [itemPatent getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPatentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```