---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb1bb9345bdb36423b732245427883388996d3b1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412612"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personCertificationId := "personCertification-id"
result, err := graphClient.UsersById(&userId).Profile().CertificationsById(&personCertificationId).Delete(nil)


```