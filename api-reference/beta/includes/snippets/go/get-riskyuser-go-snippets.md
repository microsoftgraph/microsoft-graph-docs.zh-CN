---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 827e018dfe91df4ee0918864e5760558573d0995
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

riskyUserId := "riskyUser-id"
result, err := graphClient.TenantRelationships().ManagedTenants().RiskyUsersById(&riskyUserId).Get(options);


```