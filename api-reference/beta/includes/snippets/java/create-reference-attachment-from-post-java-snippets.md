---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87bf2adb16bfa8f208c2fa206f7d576f864578c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876011"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.referenceAttachment"));
attachment.name = "Personal pictures";
attachment.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachment.providerType = "oneDriveConsumer";
attachment.permission = "Edit";
attachment.isFolder = "True";

graphClient.groups("c75831bdfad").threads("AAQkAGF97XEKhULw").posts("AAMkAGFcAAA").attachments()
    .buildRequest()
    .post(attachment);

```