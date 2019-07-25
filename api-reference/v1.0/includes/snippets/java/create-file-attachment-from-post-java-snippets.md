---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f7eeb7c9f28036cf5f4f1800aa7087a9f74c5b58
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888692"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachment.name = "name-value";
attachment.contentBytes = "base64-contentBytes-value";

graphClient.groups("{id}").threads("{id}").posts("{id}").attachments()
    .buildRequest()
    .post(attachment);

```