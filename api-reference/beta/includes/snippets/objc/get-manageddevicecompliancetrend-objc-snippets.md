---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bbb1d00ed7586c41ff8ffeb7e59d3e17e954c7894307beae1c45a4ae6457ec4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274364"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphManagedDeviceComplianceTrend *managedDeviceComplianceTrend = [[MSGraphManagedDeviceComplianceTrend alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```