---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca86bfe9f9dad05e814cc75f69ef55d0316971eb38618a96a40fb905d05e5f2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("84b80893-8749-40a3-97b7-68513b600544");
idsList.add("5d6059b6-368d-45f8-91e1-8e07d485f1d0");

LinkedList<String> typesList = new LinkedList<String>();
typesList.add("user");

graphClient.directoryObjects()
    .getByIds(DirectoryObjectGetByIdsParameterSet
        .newBuilder()
        .withIds(idsList)
        .withTypes(typesList)
        .build())
    .buildRequest()
    .post();

```