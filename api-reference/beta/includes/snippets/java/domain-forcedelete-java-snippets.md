---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5082607a4bf7bbf58de3bc88518d14fb46ac4a98
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956046"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean disableUserAccounts = true;

graphClient.domains("contoso.com")
    .forceDelete(disableUserAccounts)
    .buildRequest()
    .post();

```