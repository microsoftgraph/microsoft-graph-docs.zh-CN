---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 894c82853b9a2ffa0740cc6e4e3c4f693cf85d43
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975678"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).Get(options)


```