---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afd51189f8806403cdd3298068db4564b17d9532
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329129"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
serviceAnnouncementAttachmentId := "serviceAnnouncementAttachment-id"
graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).AttachmentsById(&serviceAnnouncementAttachmentId).Content().Get()


```