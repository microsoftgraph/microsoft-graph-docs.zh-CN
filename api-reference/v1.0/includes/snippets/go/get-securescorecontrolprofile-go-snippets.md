---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79eab2457509c84ca5fd55541bafd46bd57515c4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088878"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

secureScoreControlProfileId := "secureScoreControlProfile-id"
result, err := graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Get(options)


```