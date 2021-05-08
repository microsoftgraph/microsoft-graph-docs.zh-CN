---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e28ec53450f992d263cf3192df4deb61dbe23e1
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240688"
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