---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97d1a09475a22f89684ce6da94017284f3cd0f27
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcSnapshotId := "cloudPcSnapshot-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().SnapshotsById(&cloudPcSnapshotId).Get()


```