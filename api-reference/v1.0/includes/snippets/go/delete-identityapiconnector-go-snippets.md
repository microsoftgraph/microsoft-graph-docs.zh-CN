---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c426075e0a19a25ad2e97e083139092c02b8a761
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288221"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityApiConnectorId := "identityApiConnector-id"
graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Delete(nil)


```