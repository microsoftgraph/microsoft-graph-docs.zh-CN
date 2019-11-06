---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea76314dc01cbfb66d8d51b2da4308e5b76ab33
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994270"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *accessPackageResourceList = [[NSMutableArray alloc] init];
        accessPackageResourceList = [jsonFinal valueForKey:@"value"];
        MSGraphAccessPackageResource *accessPackageResource = [[MSGraphAccessPackageResource alloc] initWithDictionary:[accessPackageResourceList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```