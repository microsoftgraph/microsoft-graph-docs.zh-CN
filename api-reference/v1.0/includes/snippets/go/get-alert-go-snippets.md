---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9e7d6a5d5cad11ad2d0ef29b2e1d687287e26e2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103190"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

alertId := "alert-id"
result, err := graphClient.Security().AlertsById(&alertId).Get(options)


```