---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 686d516628223cc44cc7e126eb22eefd5b9f460f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachment.name = "smile";
attachment.contentBytes = "base64R0lGODdhEAYEAA7";

graphClient.me().messages("AAMkpsDRVK").attachments()
    .buildRequest()
    .post(attachment);

```