---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f5a9b14b24a684aa6430de4ee3fd684b558a369
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318139"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveActivityUserDetailList = [[NSMutableArray alloc] init];
        oneDriveActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveActivityUserDetail *oneDriveActivityUserDetail = [[MSGraphOneDriveActivityUserDetail alloc] initWithDictionary:[oneDriveActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```