---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bb7c44411d7c9856d5eafebcd70e228497b0a1e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

skillProficiencyId := "skillProficiency-id"
graphClient.Me().Profile().SkillsById(&skillProficiencyId).Delete(options)


```