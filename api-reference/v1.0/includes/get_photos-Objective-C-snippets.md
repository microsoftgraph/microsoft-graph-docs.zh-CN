---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05b01e3b9dbd395e39871d01472295e8b1c5cfbb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314590"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/photos"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *profilePhotoList = [[NSMutableArray alloc] init];
        profilePhotoList = [jsonFinal valueForKey:@"value"];
        MSGraphProfilePhoto *profilePhoto = [[MSGraphProfilePhoto alloc] initWithDictionary:[profilePhotoList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```