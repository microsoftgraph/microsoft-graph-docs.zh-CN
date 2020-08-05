---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11398468a5843e34b0d9933aeac5eb1c569ccd73
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566643"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/profileCardProperties"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProfileCardProperty *profileCardProperty = [[MSGraphProfileCardProperty alloc] init];
[profileCardProperty setDirectoryPropertyName:@"CustomAttribute1"];
NSMutableArray *annotationsList = [[NSMutableArray alloc] init];
MSGraphProfileCardAnnotation *annotations = [[MSGraphProfileCardAnnotation alloc] init];
[annotations setDisplayName:@"Cost Center"];
NSMutableArray *localizationsList = [[NSMutableArray alloc] init];
MSGraphDisplayNameLocalization *localizations = [[MSGraphDisplayNameLocalization alloc] init];
[localizations setLanguageTag:@"ru-RU"];
[localizations setDisplayName:@"центр затрат"];
[localizationsList addObject: localizations];
[annotations setLocalizations:localizationsList];
[annotationsList addObject: annotations];
[profileCardProperty setAnnotations:annotationsList];

NSError *error;
NSData *profileCardPropertyData = [profileCardProperty getSerializedDataWithError:&error];
[urlRequest setHTTPBody:profileCardPropertyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```