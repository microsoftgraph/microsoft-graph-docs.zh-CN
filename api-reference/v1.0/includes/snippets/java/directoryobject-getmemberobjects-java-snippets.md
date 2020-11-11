---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c14360127558e5be4d058d35953546f97dd5fb7f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.directoryObjects("{object-id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```