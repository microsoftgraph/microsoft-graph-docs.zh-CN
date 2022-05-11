---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dec5ea4bd37a48105da8e5f5e99fdfb89a3ed045
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329137"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

placeId := "place-id"
result, err := graphClient.PlacesById(&placeId).Get()


```