---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75bf5e62d1eacb4e1c54e371e363fd38b43b6c20
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442852"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/updatableAssets/unenrollAssets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphWindowsUpdatesUpdateCategory *updateCategory = [MSGraphWindowsUpdatesUpdateCategory feature];
payloadDictionary[@"updateCategory"] = updateCategory;

NSMutableArray *assetsList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesUpdatableAsset *assets = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];
[assets setId:@"String (identifier)"];
[assetsList addObject: assets];
payloadDictionary[@"assets"] = assetsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```