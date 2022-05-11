---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1c3ed8d2f31ecca4198bf42b8328366df0b705d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326840"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Delete()


```