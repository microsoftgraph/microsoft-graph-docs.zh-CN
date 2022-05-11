---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0bdb87a2705bc8401418cc4cefdd04517f80338
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

informationProtectionLabelId := "informationProtectionLabel-id"
result, err := graphClient.Me().InformationProtection().Policy().LabelsById(&informationProtectionLabelId).Get()


```