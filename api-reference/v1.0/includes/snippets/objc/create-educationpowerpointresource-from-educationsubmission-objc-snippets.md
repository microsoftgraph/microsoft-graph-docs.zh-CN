---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03075e381f8fe18a9d184877c44ddfd64c843c0c
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560448"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationSubmissionResource *educationSubmissionResource = [[MSGraphEducationSubmissionResource alloc] init];
MSGraphEducationResource *resource = [[MSGraphEducationResource alloc] init];
[resource setDisplayName:@"state diagram.pptx"];
[resource setFileUrl:@"https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2"];
[educationSubmissionResource setResource:resource];

NSError *error;
NSData *educationSubmissionResourceData = [educationSubmissionResource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationSubmissionResourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```