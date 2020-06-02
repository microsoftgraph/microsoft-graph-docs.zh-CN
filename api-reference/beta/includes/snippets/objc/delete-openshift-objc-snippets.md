---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e70ea96e8f2807e5e5a706581bc7d77934c9298d
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219214"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]]];
[urlRequest setHTTPMethod:@"DELETE"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```