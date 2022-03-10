---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcf2e706cb0aa978af35878ee1fb87897ce26d1a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411805"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

securityActionId := "securityAction-id"
graphClient.Security().SecurityActionsById(&securityActionId).CancelSecurityAction(securityAction-id).Post(nil)


```