---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68830a0addabe4fa286076fb96b3ab69b3081602
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201216"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.administrativeUnits("{id}").members().references()
    .buildRequest()
    .post(directoryObject);

```