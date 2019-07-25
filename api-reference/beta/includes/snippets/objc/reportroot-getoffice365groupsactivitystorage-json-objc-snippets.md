---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ad958cb2fb697a647ac5ad9d3eae7ff1e7c41ed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727260"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityStorageList = [[NSMutableArray alloc] init];
        office365GroupsActivityStorageList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityStorage *office365GroupsActivityStorage = [[MSGraphOffice365GroupsActivityStorage alloc] initWithDictionary:[office365GroupsActivityStorageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```