---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43891593fddf0f6880e2abfb8555a351cee27886
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978061"
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