---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d031ca1450e0a43ea05532c0e08140eb61a9872
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948117"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/connectors/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintConnector *printConnector = [[MSGraphPrintConnector alloc] init];
[printConnector setName:@"ConnectorName"];
[printConnector setFullyQualifiedDomainName:@"CONNECTOR-MACHINE"];
[printConnector setOperatingSystem:@"Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555"];
[printConnector setAppVersion:@"0.19.7338.23496"];
MSGraphPrinterLocation *location = [[MSGraphPrinterLocation alloc] init];
[location setLatitude: 1.1];
[location setLongitude: 2.2];
[location setAltitudeInMeters: 3];
[printConnector setLocation:location];

NSError *error;
NSData *printConnectorData = [printConnector getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printConnectorData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```