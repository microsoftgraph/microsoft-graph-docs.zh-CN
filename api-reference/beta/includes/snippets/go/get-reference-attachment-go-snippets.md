---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f6ba928f483045bde9c58f37a0eaf0eb8e42ca
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Get(options)


```