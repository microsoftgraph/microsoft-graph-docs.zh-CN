---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ce6e2f89e68a5ba12c3640c79acd7247e15c760
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981202"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemPublicationId := "itemPublication-id"
result, err := graphClient.Me().Profile().PublicationsById(&itemPublicationId).Get(options)


```