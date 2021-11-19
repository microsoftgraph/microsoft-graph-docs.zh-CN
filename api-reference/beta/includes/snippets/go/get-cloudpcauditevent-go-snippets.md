---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea49596af6f51f83d687d9728b9b471c0e74748b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcAuditEventId := "cloudPcAuditEvent-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().AuditEventsById(&cloudPcAuditEventId).Get(options)


```