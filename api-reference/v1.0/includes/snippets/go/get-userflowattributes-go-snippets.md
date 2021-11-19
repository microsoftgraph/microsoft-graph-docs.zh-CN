---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c53788d541f094a03c2fd52e0bef33b7fab27cd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowAttributeId := "identityUserFlowAttribute-id"
result, err := graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Get(options)


```