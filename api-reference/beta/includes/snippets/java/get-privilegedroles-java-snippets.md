---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d5db62969e03cb0f1ee4b3408b270757047258d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970407"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleCollectionPage privilegedRoles = graphClient.privilegedRoles()
    .buildRequest()
    .get();

```