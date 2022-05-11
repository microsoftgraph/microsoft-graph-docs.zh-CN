---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eac1e25ee1c48ded9bab155ae7bd940267fbfa67
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329134"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programControlId := "programControl-id"
graphClient.ProgramControlsById(&programControlId).Delete()


```