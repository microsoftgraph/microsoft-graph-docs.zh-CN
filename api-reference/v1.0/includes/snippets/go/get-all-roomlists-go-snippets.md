---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf90e86ee7db00c6d8c07d05852cf35995ee924
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289196"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

placeId := "place-id"
result, err := graphClient.PlacesById(&placeId).Get(nil)


```