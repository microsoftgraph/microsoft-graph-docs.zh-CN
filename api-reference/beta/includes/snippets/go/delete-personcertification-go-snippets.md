---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ed729c379d5c2f68c1e2d14e64b770b430f61fc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103218"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personCertificationId := "personCertification-id"
graphClient.UsersById(&userId).Profile().CertificationsById(&personCertificationId).Delete(options)


```