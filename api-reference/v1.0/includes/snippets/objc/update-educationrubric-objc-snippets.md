---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0935e2923ab5735b0ee7a9110f31297ec446dace5f6e6cebde80fc4ee22f7232
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104989"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationRubric *educationRubric = [[MSGraphEducationRubric alloc] init];
[educationRubric setDisplayName:@"Example Credit Rubric after display name patch"];

NSError *error;
NSData *educationRubricData = [educationRubric getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationRubricData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```