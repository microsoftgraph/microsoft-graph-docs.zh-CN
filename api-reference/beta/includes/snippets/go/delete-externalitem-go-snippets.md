---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcfd41025cec1447aab6b8172ec35da23b9ffd3e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394402"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Delete(nil)


```