---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fba65c0fdb013e6667504040ac572cff29b36ad4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998972"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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