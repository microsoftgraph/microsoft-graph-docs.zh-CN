---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2134c84c788e93f19b017cee1c7e5e09e77febf6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956295"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "2c891f12-928d-4da2-8d83-7d2434a0d8dc";

graphClient.directoryRoles("0afed502-2456-4fd4-988e-3c21924c28a7").members().references()
    .buildRequest()
    .post(directoryObject);

```