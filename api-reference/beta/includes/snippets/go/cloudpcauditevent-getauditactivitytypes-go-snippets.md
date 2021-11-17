---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74bf15c4ea10c631a46abff76021b2ce87416dd4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003449"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcAuditEventId := "cloudPcAuditEvent-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().AuditEventsById(&cloudPcAuditEventId).Get(options)


```