---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f7a4144ec12923229250276f159ccfd2ce2ee4b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412079"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).UnsetVerifiedPublisher(application-id).Post(nil)


```