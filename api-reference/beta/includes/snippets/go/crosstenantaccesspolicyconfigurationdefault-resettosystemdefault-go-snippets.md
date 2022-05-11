---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3715d3a0c076083e20920bd78d05451653d1a2f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

graphClient.Policies().CrossTenantAccessPolicy().Default().ResetToSystemDefault().Post()


```