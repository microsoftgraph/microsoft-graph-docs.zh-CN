---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3012c1802d9b4f20e6987ba4c1b7a5f6051f9f60
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136281"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationCategory *educationCategory = [[MSGraphEducationCategory alloc] init];
[educationCategory setDisplayName:@"Quizzes"];

NSError *error;
NSData *educationCategoryData = [educationCategory getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationCategoryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```