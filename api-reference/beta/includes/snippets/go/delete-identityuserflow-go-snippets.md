---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5030a45aab2ce218b2daca3c29848a3c891bd09a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
graphClient.Identity().UserFlowsById(&identityUserFlowId).Delete()


```