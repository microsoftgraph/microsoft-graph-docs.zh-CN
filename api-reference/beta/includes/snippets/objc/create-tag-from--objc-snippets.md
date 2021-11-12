---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4567934819d319143250868797d91d9672345b9016a855071b17f98da279d5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161504"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryTag *tag = [[MSGraphEdiscoveryTag alloc] init];
[tag setDisplayName:@"Privileged"];
[tag setDescription:@"The document is privileged"];

NSError *error;
NSData *tagData = [tag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```