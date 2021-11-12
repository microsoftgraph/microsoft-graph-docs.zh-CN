---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4b85267710daf19965e42face731820c82537f01b0938d98e5da5e2eee9afda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161701"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryTag *tag = [[MSGraphEdiscoveryTag alloc] init];
[tag setDescription:@"This is an updated description."];

NSError *error;
NSData *tagData = [tag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```