---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6973a99e3a2778a65d6e6e3d89f5aba912a6656c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315810"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/root/operations/contentTypeCopy,0x010100298A15181454D84EBB62EDD7559FCBFE"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRichLongRunningOperation *richLongRunningOperation = [[MSGraphRichLongRunningOperation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```