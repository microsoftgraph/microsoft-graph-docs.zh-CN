---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6302d1e676a6caf71fb81069eb652859c67ff0a2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033937"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

placeId := "place-id"
result, err := graphClient.PlacesById(&placeId).Get(options)


```