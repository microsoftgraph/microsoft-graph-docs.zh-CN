---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b15f56463f2a51f7f96ba454c1e90f6f75a4195
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Teamwork().AssociatedTeams().Get()


```