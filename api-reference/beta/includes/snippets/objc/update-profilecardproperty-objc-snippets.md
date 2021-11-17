---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15b6103a23cef675a7e930c8b67646a0903f74c3921373d3afee8824b4afd780
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162177"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphProfileCardProperty *profileCardProperty = [[MSGraphProfileCardProperty alloc] init];
NSMutableArray *annotationsList = [[NSMutableArray alloc] init];
MSGraphProfileCardAnnotation *annotations = [[MSGraphProfileCardAnnotation alloc] init];
NSMutableArray *localizationsList = [[NSMutableArray alloc] init];
MSGraphDisplayNameLocalization *localizations = [[MSGraphDisplayNameLocalization alloc] init];
[localizations setLanguageTag:@"no-NB"];
[localizations setDisplayName:@"Kostnads Senter"];
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