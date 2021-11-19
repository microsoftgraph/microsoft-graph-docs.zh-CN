---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6bcf819858d8b856f3fb38b210ded4579e832b1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088935"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Patch(options)


```