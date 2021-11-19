---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2ad4d5f6ae754fe55b5fdf3348a5b50e1d437b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101933"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printServiceId := "printService-id"
printServiceEndpointId := "printServiceEndpoint-id"
result, err := graphClient.Print().ServicesById(&printServiceId).EndpointsById(&printServiceEndpointId).Get(options)


```