---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72cce9d23b60ab67656064455adb784ba495098a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .delete();

```