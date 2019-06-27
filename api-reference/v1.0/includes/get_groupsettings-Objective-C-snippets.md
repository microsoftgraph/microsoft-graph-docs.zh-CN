---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f5a8caf5ef5b0f16e151583008d7acc68f379a03
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322507"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettings"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupSettingList = [[NSMutableArray alloc] init];
        groupSettingList = [jsonFinal valueForKey:@"value"];
        MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] initWithDictionary:[groupSettingList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```