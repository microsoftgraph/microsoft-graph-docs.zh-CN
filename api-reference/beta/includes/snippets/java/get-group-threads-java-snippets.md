---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa56b0b085bac8969893a1fc8be78a16a295e7b9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953836"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationThreadCollectionPage threads = graphClient.groups("{id}").threads()
    .buildRequest()
    .get();

```