---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d708572023c4aa96d64f7f5b7495e1660136db8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724134"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/licenseDetails"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *licenseDetailsList = [[NSMutableArray alloc] init];
        licenseDetailsList = [jsonFinal valueForKey:@"value"];
        MSGraphLicenseDetails *licenseDetails = [[MSGraphLicenseDetails alloc] initWithDictionary:[licenseDetailsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```