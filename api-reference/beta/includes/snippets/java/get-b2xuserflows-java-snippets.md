---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c4d9255ff6220bb40ce0fbb299d318949d90159
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961082"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = graphClient.identity().b2xUserFlows("{id}")
    .buildRequest()
    .get();

```