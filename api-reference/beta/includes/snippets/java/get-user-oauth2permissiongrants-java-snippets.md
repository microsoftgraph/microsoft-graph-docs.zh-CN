---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ad3e6837164638270661c9e68548fd7d911810a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975202"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content oauth2PermissionGrants = graphClient.users("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```