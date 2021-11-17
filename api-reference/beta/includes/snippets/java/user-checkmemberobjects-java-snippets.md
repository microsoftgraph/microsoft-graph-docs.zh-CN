---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a1f77987fa4725ea375135229d1c9e36c44a0c96a1fe4fc931f21ff8e02615a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("80a963dd-84af-4eb8-b2a6-781e444d4fb0");
idsList.add("62e90394-69f5-4237-9190-012177145e10");
idsList.add("86a64f51-3a64-4cc6-a8c8-6b8f000c0f52");
idsList.add("ac38546e-ddf3-437a-ac5c-27a94cd7a0f1");

graphClient.me()
    .checkMemberObjects(DirectoryObjectCheckMemberObjectsParameterSet
        .newBuilder()
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```