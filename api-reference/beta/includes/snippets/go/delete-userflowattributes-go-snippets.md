---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9e7a684d24f5b007c8d95a1224afc6680fbc0f5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

identityUserFlowAttributeId := "identityUserFlowAttribute-id"
graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Delete(options)


```