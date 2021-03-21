---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d609505bba73238e21b60048f286f5a306466b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978014"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("84b80893874940a3-97b7-68513b600544");
idsList.add("5d6059b6368d-45f8-91e18e07d485f1d0");

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