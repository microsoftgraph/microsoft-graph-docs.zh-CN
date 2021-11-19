---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c5bfb1c95c92aa8f46b27c39004ae6dd78e30c5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).Get(options)


```