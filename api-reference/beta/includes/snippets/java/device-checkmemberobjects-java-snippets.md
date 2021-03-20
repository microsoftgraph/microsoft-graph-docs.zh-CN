---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c86f208fc7b1966a0189be753d7d32053baed37f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971277"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("80a963dd-84af-4eb8-b2a6-781e444d4fb0");
idsList.add("62e90394-69f5-4237-9190-012177145e10");
idsList.add("86a64f51-3a64-4cc6-a8c8-6b8f000c0f52");
idsList.add("ac38546e-ddf3-437a-ac5c-27a94cd7a0f1");

graphClient.devices("{id}")
    .checkMemberObjects(DirectoryObjectCheckMemberObjectsParameterSet
        .newBuilder()
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```