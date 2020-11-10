---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f1c9fb706c23cfbb816f982143096df4bec2232
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954830"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.me().events("{id}").attachments()
    .buildRequest()
    .get();

```