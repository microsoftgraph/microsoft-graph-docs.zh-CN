---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd96591eaf2ed7ebd9a48f48428d5f99f958f3a7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500569"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/anniversaries/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnnualEvent *personAnnualEvent = [[MSGraphPersonAnnualEvent alloc] init];
[personAnnualEvent setAllowedAudiences: [MSGraphAllowedAudiences contacts]];

NSError *error;
NSData *personAnnualEventData = [personAnnualEvent getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnnualEventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```