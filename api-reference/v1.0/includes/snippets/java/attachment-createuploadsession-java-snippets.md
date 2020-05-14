---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e49dfadc6b753a4c34122adc622f0478a5d53428
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052382"
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