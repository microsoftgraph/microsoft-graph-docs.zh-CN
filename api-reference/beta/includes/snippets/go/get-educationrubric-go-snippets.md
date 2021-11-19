---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad2be67a98e269130b2de90a926448cee41d4ae8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100605"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
result, err := graphClient.Education().Me().RubricsById(&educationRubricId).Get(options)


```