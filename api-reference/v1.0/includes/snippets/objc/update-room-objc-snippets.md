---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 487198d434868fbea98f155bbc63097303ba70bb
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336363"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/places/cf100@contoso.com"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlace *place = [[MSGraphPlace alloc] init];
[place setNickname:@"Conf Room"];
[place setBuilding:@"1"];
[place setLabel:@"100"];
[place setCapacity:@"50"];
[place setIsWheelchairAccessible: false];

NSError *error;
NSData *placeData = [place getSerializedDataWithError:&error];
[urlRequest setHTTPBody:placeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```