---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccb4c80c38662fbc736194f88f1a3aecd3ac37b1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090371"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityApiConnectorId := "identityApiConnector-id"
graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).Delete(options)


```