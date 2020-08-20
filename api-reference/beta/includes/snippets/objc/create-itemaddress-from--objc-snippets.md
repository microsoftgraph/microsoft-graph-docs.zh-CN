---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2b9c53093a355ff66e92c585f9eb85a2d4fef12
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820218"
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