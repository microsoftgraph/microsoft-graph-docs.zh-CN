---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 940586718bc894c7a5f7e66cb1ad39a0d93327a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776989"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/connectors/{printConnectorId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintConnector *printConnector = [[MSGraphPrintConnector alloc] init];
[printConnector setDisplayName:@"ConnectorName"];
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