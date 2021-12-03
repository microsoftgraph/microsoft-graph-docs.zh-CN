---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 026cdc01aaaea8ee450ac42f6e980aba7f2372b9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288131"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Delete(nil)


```