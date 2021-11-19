---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8222950cdafcd53a6a1be463928f48a20fe612d9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

secureScoreId := "secureScore-id"
result, err := graphClient.Security().SecureScoresById(&secureScoreId).Get(options)


```