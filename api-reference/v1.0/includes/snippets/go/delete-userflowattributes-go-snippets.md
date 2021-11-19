---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a9292c2dcb29e8986311f6fcbbcee7d9e24d796
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowAttributeId := "identityUserFlowAttribute-id"
graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Delete(options)


```