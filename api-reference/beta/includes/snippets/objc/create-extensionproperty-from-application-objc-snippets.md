---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 254cfa4d6932a74246525de27cf1e678715cff45293a3797260a626bf84f8caa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161309"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/extensionProperties"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExtensionProperty *extensionProperty = [[MSGraphExtensionProperty alloc] init];
[extensionProperty setName:@"extensionName"];
[extensionProperty setDataType:@"string"];
NSMutableArray *targetObjectsList = [[NSMutableArray alloc] init];
[targetObjectsList addObject: @"Application"];
[extensionProperty setTargetObjects:targetObjectsList];

NSError *error;
NSData *extensionPropertyData = [extensionProperty getSerializedDataWithError:&error];
[urlRequest setHTTPBody:extensionPropertyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```