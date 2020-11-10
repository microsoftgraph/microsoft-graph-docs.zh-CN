---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b3b16fe9c461e755da01d22c8428f9dacf9f4cb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980068"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.servicePrincipals("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```