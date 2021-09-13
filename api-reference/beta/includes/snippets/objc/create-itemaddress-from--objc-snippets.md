---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05c4050ffd74e394c4af87309763a18efa96e05fb2fbbd648ec848d86afef5a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333726"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/addresses"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemAddress *itemAddress = [[MSGraphItemAddress alloc] init];
[itemAddress setDisplayName:@"Home"];
MSGraphPhysicalAddress *detail = [[MSGraphPhysicalAddress alloc] init];
[detail setType: [MSGraphPhysicalAddressType home]];
[detail setPostOfficeBox: null];
[detail setStreet:@"221B Baker Street"];
[detail setCity:@"London"];
[detail setState: null];
[detail setCountryOrRegion:@"United Kingdom"];
[detail setPostalCode:@"E14 3TD"];
[itemAddress setDetail:detail];

NSError *error;
NSData *itemAddressData = [itemAddress getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemAddressData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```