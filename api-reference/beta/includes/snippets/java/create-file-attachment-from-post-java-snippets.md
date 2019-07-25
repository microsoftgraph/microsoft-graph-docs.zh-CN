---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 10efb1e5ee21cad141c715218e7c08b982f2f254
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachment.name = "name-value";
attachment.contentBytes = "contentBytes-value";

graphClient.groups("{id}").threads("{id}").posts("{id}").attachments()
    .buildRequest()
    .post(attachment);

```