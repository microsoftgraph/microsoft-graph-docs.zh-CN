---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61c540825278dc46cbb5d9dc2b797b8002bf86fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520634"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/settings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directorySettingList = [[NSMutableArray alloc] init];
        directorySettingList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectorySetting *directorySetting = [[MSGraphDirectorySetting alloc] initWithDictionary:[directorySettingList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```