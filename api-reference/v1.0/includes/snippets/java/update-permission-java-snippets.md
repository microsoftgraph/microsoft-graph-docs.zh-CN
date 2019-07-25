---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 161a0a2b032ba6c31ace951218ba41e1953e70f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885059"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = new Permission();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("read");
permission.roles = rolesList;

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .patch(permission);

```