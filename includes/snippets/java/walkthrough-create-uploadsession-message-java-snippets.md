---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79dbefa1fd4a442d473d252d91879514ffc551a2f6285178d7d2cd653ba64513
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240409"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322;

graphClient.me().messages("AAMkADI5MAAIT3drCAAA=").attachments()
    .createUploadSession(attachmentItem)
    .buildRequest()
    .post();

```