---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ca1780fff880412547349d2ac4603569b52732a1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881794"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.me().drive().root().subscriptions("socketIo")
    .buildRequest()
    .get();

```