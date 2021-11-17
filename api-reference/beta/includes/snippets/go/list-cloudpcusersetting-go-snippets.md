---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f69a099f0d759bdd14498f1e4e1c7290ef659850
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.DeviceManagement().VirtualEndpoint().UserSettings().Get(options)


```