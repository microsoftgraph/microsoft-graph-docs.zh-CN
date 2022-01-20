---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccf4d00a5e4b842ec37ad7101d6f3e107a77af43
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().GetAllMessages()().Get(nil)


```