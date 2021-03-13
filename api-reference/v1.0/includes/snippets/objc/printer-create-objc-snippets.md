---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b97b8798bee8c41c0ca34d361187e4ac6270f47
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772063"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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