---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68830a0addabe4fa286076fb96b3ab69b3081602
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890218"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.administrativeUnits("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```