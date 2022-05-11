---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90d3a3cddb0895e409eed9f9f21068ab7eb323de
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326362"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.TermStore().GroupsById(&groupId).Delete()


```