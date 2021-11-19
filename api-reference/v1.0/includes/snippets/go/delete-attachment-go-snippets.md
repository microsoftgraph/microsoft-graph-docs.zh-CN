---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 897bca3e7b36343d5d926bd3bed9286f616c3fc7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099395"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
attachmentId := "attachment-id"
graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Delete(options)


```