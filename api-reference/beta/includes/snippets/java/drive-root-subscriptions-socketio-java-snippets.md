---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca1780fff880412547349d2ac4603569b52732a1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982233"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.me().drive().root().subscriptions("socketIo")
    .buildRequest()
    .get();

```