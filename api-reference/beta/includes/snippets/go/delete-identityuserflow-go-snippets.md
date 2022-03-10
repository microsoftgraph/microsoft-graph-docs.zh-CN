---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de45d9a68f7531d19cf9da07d30ee9c50db61dba
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412248"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
result, err := graphClient.Identity().UserFlowsById(&identityUserFlowId).Delete(nil)


```