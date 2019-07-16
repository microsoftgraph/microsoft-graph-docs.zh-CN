---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05b01e3b9dbd395e39871d01472295e8b1c5cfbb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735984"
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