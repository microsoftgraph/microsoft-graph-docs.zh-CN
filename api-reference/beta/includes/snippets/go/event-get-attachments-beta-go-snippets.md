---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d808749716c0f0538649ae0250c008a43f5b6a08
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326274"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Get()


```