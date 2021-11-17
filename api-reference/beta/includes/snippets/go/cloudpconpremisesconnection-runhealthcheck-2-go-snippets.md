---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75c65494f0e55b5e1567e6f1d43ae3df4f20e485
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987173"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcOnPremisesConnectionId := "cloudPcOnPremisesConnection-id"
graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnectionsById(&cloudPcOnPremisesConnectionId).RunHealthChecks().Post(options)


```