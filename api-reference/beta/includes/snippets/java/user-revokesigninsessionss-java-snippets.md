---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 224cb4e041c09e2d2f4c87cb73521da6c1e349b0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978828"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .revokeSignInSessions()
    .buildRequest()
    .post();

```