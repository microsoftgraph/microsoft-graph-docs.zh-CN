---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa5e1a2f81dd33a2039159746a7bb6483599a073
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130157"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/columns"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphColumnDefinition *columnDefinition = [[MSGraphColumnDefinition alloc] init];
[columnDefinition setDescription:@"test"];
[columnDefinition setEnforceUniqueValues: false];
[columnDefinition setHidden: false];
[columnDefinition setIndexed: false];
[columnDefinition setName:@"Title"];
MSGraphTextColumn *text = [[MSGraphTextColumn alloc] init];
[text setAllowMultipleLines: false];
[text setAppendChangesToExistingText: false];
[text setLinesForEditing: 0];
[text setMaxLength: 255];
[columnDefinition setText:text];

NSError *error;
NSData *columnDefinitionData = [columnDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:columnDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```