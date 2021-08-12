---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65d6602339c6767bcb950d3fdce61b6d952811c66eeb6ef93a56e34a727659bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240412"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322;

graphClient.me().events("AAMkADU5CCmSAAA=").attachments()
    .createUploadSession(attachmentItem)
    .buildRequest()
    .post();

```