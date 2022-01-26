---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 927e9e1459947184844305a7bf280686d931fb9d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225784"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
serviceAnnouncementAttachmentId := "serviceAnnouncementAttachment-id"
graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).AttachmentsById(&serviceAnnouncementAttachmentId).Content().Get(nil)


```