---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 807f83f43f763bfdd9f3cbef0d7eb8d8149ebc139d7650845d716292adbaf5e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103845"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/settings/regionalAndLanguageSettings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRegionalAndLanguageSettings *regionalAndLanguageSettings = [[MSGraphRegionalAndLanguageSettings alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```