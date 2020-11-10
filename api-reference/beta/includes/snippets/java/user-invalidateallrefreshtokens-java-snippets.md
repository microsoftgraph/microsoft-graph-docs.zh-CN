---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9a2a0f07f72f3f6a347ba31c2b93a1118e3450b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973820"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .invalidateAllRefreshTokens()
    .buildRequest()
    .post();

```