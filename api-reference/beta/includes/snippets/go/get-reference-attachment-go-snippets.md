---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da337f27b74fccf5ea88c5deb049e97ee5d6dd44
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327146"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Get()


```