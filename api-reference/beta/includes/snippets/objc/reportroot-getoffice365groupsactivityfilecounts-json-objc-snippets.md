---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c09beaf2e65ea5bdabac0236d702b6f5c14de800
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727343"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityFileCountsList = [[NSMutableArray alloc] init];
        office365GroupsActivityFileCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityFileCounts *office365GroupsActivityFileCounts = [[MSGraphOffice365GroupsActivityFileCounts alloc] initWithDictionary:[office365GroupsActivityFileCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```