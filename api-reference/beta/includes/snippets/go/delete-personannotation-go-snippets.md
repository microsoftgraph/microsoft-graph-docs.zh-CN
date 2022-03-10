---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7308d4ff12c3947b9fa5a14af2284989e25ca13
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personAnnotationId := "personAnnotation-id"
result, err := graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Delete(nil)


```