---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec04d9d282bdd9a574af942a166413f1555ec16b
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629806"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/05aa6a98-956a-45c0-b13b-88076a23f2cd/settings/a06fa228-3042-4662-bd09-33e298da1afe"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```