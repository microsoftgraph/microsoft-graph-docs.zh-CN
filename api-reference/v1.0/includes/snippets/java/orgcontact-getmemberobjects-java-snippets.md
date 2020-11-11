---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 043fd9a8df56d98a4fd6ba47c390fde94100d309
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984169"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.contacts("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```