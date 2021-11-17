---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc38cccc1339f468bddeaadf22443a1b87448ce7ba87d3c5fedf1b4eab94df0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902479"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSwapShiftsChangeRequest *swapShiftsChangeRequest = [[MSGraphSwapShiftsChangeRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```