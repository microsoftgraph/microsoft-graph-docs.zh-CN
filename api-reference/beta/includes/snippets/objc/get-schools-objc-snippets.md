---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c9ae09612e9d2402064d83e4a6bccd9a75d55dd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521257"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/schools"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationSchoolList = [[NSMutableArray alloc] init];
        educationSchoolList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationSchool *educationSchool = [[MSGraphEducationSchool alloc] initWithDictionary:[educationSchoolList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```