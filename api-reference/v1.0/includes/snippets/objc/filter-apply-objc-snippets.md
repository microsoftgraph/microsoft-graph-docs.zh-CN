---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ec497a521cccefcf00fa98ee284765c2bf10e1ce2837b0a86374567903de9bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106470"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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