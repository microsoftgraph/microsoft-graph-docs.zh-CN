---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b343d3757a5333c34558032d756770b57777aef7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

informationProtectionLabelId := "informationProtectionLabel-id"
result, err := graphClient.Me().InformationProtection().Policy().LabelsById(&informationProtectionLabelId).Get(nil)


```