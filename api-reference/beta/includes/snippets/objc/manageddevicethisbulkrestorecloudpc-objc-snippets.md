---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e713dfc096d9a5073947ed9b73ef44efb87a822c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338190"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/managedDevices/bulkRestoreCloudPc"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *managedDeviceIdsList = [[NSMutableArray alloc] init];
[managedDeviceIdsList addObject: @"30d0e128-de93-41dc-89ec-33d84bb662a0"];
[managedDeviceIdsList addObject: @"7c82a3e3-9459-44e4-94d9-b92f93bf78dd"];
payloadDictionary[@"managedDeviceIds"] = managedDeviceIdsList;

NSString *restorePointDateTimeDateTimeString = @"09/23/2021 04:00:00";
NSDate *restorePointDateTime = [NSDate ms_dateFromString: restorePointDateTimeDateTimeString];
payloadDictionary[@"restorePointDateTime"] = restorePointDateTime;

MSGraphRestoreTimeRange *timeRange = [MSGraphRestoreTimeRange before];
payloadDictionary[@"timeRange"] = timeRange;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```