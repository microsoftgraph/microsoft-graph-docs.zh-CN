---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7850ac16aedcd5cd9e30bb928e90252a12e7fb4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982950"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.groups("{group-id}").members().references()
    .buildRequest()
    .post(directoryObject);

```