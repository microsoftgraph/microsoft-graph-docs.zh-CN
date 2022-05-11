---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bc532b1f362edfb680a0078973e1b47689536f7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPublicationId := "itemPublication-id"
graphClient.Me().Profile().PublicationsById(&itemPublicationId).Delete()


```