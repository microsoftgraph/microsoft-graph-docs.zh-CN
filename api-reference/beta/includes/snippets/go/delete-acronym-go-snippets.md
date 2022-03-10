---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db138b7f2cccd565f82a9de1b9be5ed2bd2f9d54
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412493"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

acronymId := "acronym-id"
result, err := graphClient.Search().AcronymsById(&acronymId).Delete(nil)


```