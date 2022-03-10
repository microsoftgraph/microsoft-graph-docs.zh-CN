---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bff2bf443260c61ed03e7d915b638284fb98c883
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412372"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).ExtensionProperties().Delete(nil)


```