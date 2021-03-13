---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33226aef8db09d4964b35ed321b9df1869f96533
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773814"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoverySourceCollection *sourceCollection = [[MSGraphEdiscoverySourceCollection alloc] init];
[sourceCollection setDisplayName:@"Quarterly Financials search"];
[sourceCollection setContentQuery:@"subject:'Quarterly Financials'"];

NSError *error;
NSData *sourceCollectionData = [sourceCollection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:sourceCollectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```