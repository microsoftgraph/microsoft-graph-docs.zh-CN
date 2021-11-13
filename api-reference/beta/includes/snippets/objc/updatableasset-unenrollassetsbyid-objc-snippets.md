---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf54453fd4fbfcf701cd38b80f3d8c07d8b214f4bb32ff71d81d1b9b3211100e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333307"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/updatableAssets/unenrollAssetsById"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphWindowsUpdatesUpdateCategory *updateCategory = [MSGraphWindowsUpdatesUpdateCategory feature];
payloadDictionary[@"updateCategory"] = updateCategory;

NSString *memberEntityType = @"#microsoft.graph.windowsUpdates.azureADDevice";
payloadDictionary[@"memberEntityType"] = memberEntityType;

NSMutableArray *idsList = [[NSMutableArray alloc] init];
[idsList addObject: @"String"];
[idsList addObject: @"String"];
[idsList addObject: @"String"];
payloadDictionary[@"ids"] = idsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```