---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c164653f079937b100a63d7baeb5f12f87e1eef6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315544"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphWorkbookFilterCriteria *criteria = [[MSGraphWorkbookFilterCriteria alloc] init];
[criteria setCriterion1:@"criterion1-value"];
[criteria setCriterion2:@"criterion2-value"];
[criteria setColor:@"color-value"];
MSGraphString *operator = [[MSGraphString alloc] init];
[criteria setOperator:operator];
MSGraphWorkbookIcon *icon = [[MSGraphWorkbookIcon alloc] init];
[icon setSet:@"set-value"];
[icon setIndex: 99];
[criteria setIcon:icon];
[criteria setDynamicCriteria:@"dynamicCriteria-value"];
MSGraphJson *values = [[MSGraphJson alloc] init];
[criteria setValues:values];
[criteria setFilterOn:@"filterOn-value"];
payloadDictionary[@"criteria"] = criteria;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```