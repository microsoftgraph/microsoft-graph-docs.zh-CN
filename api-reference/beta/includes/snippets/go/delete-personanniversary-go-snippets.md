---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a64c8e95757ebfdee4dc3afa242e9cf8493ef4e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411744"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAnnualEventId := "personAnnualEvent-id"
result, err := graphClient.Me().Profile().AnniversariesById(&personAnnualEventId).Delete(nil)


```