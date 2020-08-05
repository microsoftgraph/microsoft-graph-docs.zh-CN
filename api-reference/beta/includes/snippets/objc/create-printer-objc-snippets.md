---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eec441d1cc60361f9bba4572daab10170d9e38e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566358"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/create"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *displayName = @"Test Printer";
payloadDictionary[@"displayName"] = displayName;

NSString *manufacturer = @"Test Printer Manufacturer";
payloadDictionary[@"manufacturer"] = manufacturer;

NSString *model = @"Test Printer Model";
payloadDictionary[@"model"] = model;

payloadDictionary[@"physicalDeviceId"] = physicalDeviceId;

BOOL hasPhysicalDevice = NO;
payloadDictionary[@"hasPhysicalDevice"] = hasPhysicalDevice;

MSGraphPrintCertificateSigningRequest *certificateSigningRequest = [[MSGraphPrintCertificateSigningRequest alloc] init];
[certificateSigningRequest setContent:@"{content}"];
[certificateSigningRequest setTransportKey:@"{sampleTransportKey}"];
payloadDictionary[@"certificateSigningRequest"] = certificateSigningRequest;

payloadDictionary[@"connectorId"] = connectorId;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```