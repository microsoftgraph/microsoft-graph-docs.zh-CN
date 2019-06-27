---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d3e74f403f9c9e68546884dbef4e7fa542a76073
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330307"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageAccountDetailList = [[NSMutableArray alloc] init];
        oneDriveUsageAccountDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageAccountDetail *oneDriveUsageAccountDetail = [[MSGraphOneDriveUsageAccountDetail alloc] initWithDictionary:[oneDriveUsageAccountDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```