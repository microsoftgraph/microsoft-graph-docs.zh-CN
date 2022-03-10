---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aba0eb3010b7b77a17f36e888e08b3850d7ed3d6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412681"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityApiConnectorId := "identityApiConnector-id"
result, err := graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Delete(nil)


```