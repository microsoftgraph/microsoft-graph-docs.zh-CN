---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 228ffabd304e78d427f66aa2c31320834a443917
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102110"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcConnectionId := "cloudPcConnection-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CloudPcConnectionsById(&cloudPcConnectionId).Get(options)


```