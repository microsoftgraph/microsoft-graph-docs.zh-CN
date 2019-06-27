---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ae1514e6bcd9e4757c72536f33518ca1e53192db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322630"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/special/{special-folder-name}/children"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *driveItemList = [[NSMutableArray alloc] init];
        driveItemList = [jsonFinal valueForKey:@"value"];
        MSGraphDriveItem *driveItem = [[MSGraphDriveItem alloc] initWithDictionary:[driveItemList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```