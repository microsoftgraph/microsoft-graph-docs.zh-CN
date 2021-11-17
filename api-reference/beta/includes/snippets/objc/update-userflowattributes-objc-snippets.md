---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d721d3edbc34d688b9682753ac845f1da262b3c1684bfc261fd893f92f00b7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220668"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlowAttribute *identityUserFlowAttribute = [[MSGraphIdentityUserFlowAttribute alloc] init];
[identityUserFlowAttribute setDescription:@"Your new hobby"];

NSError *error;
NSData *identityUserFlowAttributeData = [identityUserFlowAttribute getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityUserFlowAttributeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```