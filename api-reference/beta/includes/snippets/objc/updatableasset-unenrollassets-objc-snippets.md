---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 811c659335a7a8e234856c55ab00b0698eb45a2b646294f91fdf509ec1e14b85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333313"
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