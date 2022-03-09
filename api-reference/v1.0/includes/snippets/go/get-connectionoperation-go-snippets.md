---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1c5aae12fd9643d4c0ff28cfa050a851352f8af
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
connectionOperationId := "connectionOperation-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).OperationsById(&connectionOperationId).Get(nil)


```