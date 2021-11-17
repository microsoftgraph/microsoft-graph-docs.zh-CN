---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a459163b4cc6f4426d43f370d4fbc21186a98403
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981216"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemPublicationId := "itemPublication-id"
graphClient.Me().Profile().PublicationsById(&itemPublicationId).Delete(options)


```