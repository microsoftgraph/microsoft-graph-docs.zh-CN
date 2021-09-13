---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 379a82f0b751829c217978f38c701adf81be50e86075c47ddfcf1e68a1c6115e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106291"
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