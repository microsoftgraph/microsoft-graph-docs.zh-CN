---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c26bf4e2dbde554ae8bff9b315317596afc4a5fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
extensionId := "extension-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).ExtensionsById(&extensionId).Get()


```