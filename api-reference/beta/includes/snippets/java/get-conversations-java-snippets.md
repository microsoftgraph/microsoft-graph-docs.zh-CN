---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd5b6b5888aebbf6c59a271620b1938ecce873f9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965137"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationCollectionPage conversations = graphClient.groups("{id}").conversations()
    .buildRequest()
    .get();

```