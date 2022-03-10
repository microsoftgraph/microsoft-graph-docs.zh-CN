---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8d8dbe302df7b633fff3837cff7d264d2cec5a8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412480"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExtensionProperty *extensionProperty = [[MSGraphExtensionProperty alloc] init];
[extensionProperty setName:@"jobGroup"];
[extensionProperty setDataType:@"String"];
NSMutableArray *targetObjectsList = [[NSMutableArray alloc] init];
[targetObjectsList addObject: @"User"];
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