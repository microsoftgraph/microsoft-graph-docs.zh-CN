---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fe5ed898374efa417bfabb24ef99b6bae5aa028
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).GetActiveKey()(trustFrameworkKeySet-id).Get(nil)


```