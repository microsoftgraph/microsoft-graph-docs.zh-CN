---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 392d712590a20ebe66e0e0107e5b1c068cc56dec
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397209"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InformationProtection().Policy().Labels().Get(nil)


```