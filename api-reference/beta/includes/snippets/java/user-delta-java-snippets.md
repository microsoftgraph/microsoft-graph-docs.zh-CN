---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90daa0ba8a31ffb7c2dc95db6c6acf7283e73357
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979089"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest()
    .get();

```