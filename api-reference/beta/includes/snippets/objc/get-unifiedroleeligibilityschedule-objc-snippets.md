---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf529cd21625a4bc4f332b5bc4cbe7abbec55af8
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516046"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilitySchedules/313af44a-07c9-43a7-9970-5072a6b5591f"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleEligibilitySchedule *unifiedRoleEligibilitySchedule = [[MSGraphUnifiedRoleEligibilitySchedule alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```