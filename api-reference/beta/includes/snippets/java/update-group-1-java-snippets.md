---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10433dbb546d98a473c2db3a70df0f4a5cbe9750
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Contoso Life v2.0";
group.displayName = "Contoso Life Renewed";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```