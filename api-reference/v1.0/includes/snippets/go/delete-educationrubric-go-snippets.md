---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9da005be46a3425109a5394a6c8b3879a5ba054f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Delete(options)


```