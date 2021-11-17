---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c16141342eb1b0f9e8b541f8a09c5f058a9f1636
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992584"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printServiceId := "printService-id"
result, err := graphClient.Print().ServicesById(&printServiceId).Get(options)


```