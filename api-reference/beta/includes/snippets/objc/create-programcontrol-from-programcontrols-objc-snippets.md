---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 127b496e0f03eb1e09999fa6644ff23dd7f855f9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479291"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/programControls"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProgramControl *programControl = [[MSGraphProgramControl alloc] init];
[programControl setControlId:@"7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"];
[programControl setControlTypeId:@"6e4f3d20-c5c3-407f-9695-8460952bcc68"];
[programControl setProgramId:@"7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"];

NSError *error;
NSData *programControlData = [programControl getSerializedDataWithError:&error];
[urlRequest setHTTPBody:programControlData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```