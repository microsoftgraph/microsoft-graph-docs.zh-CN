---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 396757ae810402d47daa4d76330687ec164d8ad1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).EndGracePeriod().Post(options)


```