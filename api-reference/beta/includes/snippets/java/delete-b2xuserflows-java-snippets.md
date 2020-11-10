---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30f679b442ee99061544e0c7f15328935eaee1c3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961114"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("{id}")
    .buildRequest()
    .delete();

```