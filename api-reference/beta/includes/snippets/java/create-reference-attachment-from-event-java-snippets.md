---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0624197873c63ea3094eb55b07cc224699cf2bde7afac527818b420e55553f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103878"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReferenceAttachment attachment = new ReferenceAttachment();
attachment.name = "Personal pictures";
attachment.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachment.providerType = ReferenceAttachmentProvider.ONE_DRIVE_CONSUMER;
attachment.permission = ReferenceAttachmentPermission.EDIT;
attachment.isFolder = false;

graphClient.me().events("AAMkAGE1M88AADUv0uAAAG=").attachments()
    .buildRequest()
    .post(attachment);

```