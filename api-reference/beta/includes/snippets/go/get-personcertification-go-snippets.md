---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb8afff8580c6db95d5992cf52ff4ecb5bb94806
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088380"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personCertificationId := "personCertification-id"
result, err := graphClient.Me().Profile().CertificationsById(&personCertificationId).Get(options)


```