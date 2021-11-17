---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cd2dfbca1c709137d3ba78adc2ea23547540ec8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
calendarPermissionId := "calendarPermission-id"
result, err := graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Get(options)


```