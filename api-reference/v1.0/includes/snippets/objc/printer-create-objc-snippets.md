---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d540c50563d63fde7dc8853901cf3fe051dc6dbf743fbca1187613bce9395d9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103906"
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