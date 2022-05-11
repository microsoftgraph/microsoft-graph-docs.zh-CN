---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded64d6f47191ca087d780aacc8efeacbb33a706
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personNameId := "personName-id"
result, err := graphClient.Me().Profile().NamesById(&personNameId).Get()


```