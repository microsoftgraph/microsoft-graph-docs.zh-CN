---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa1ecf08f9abf837294f2a09d64e9ae5e7e39726
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965708"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.id = "contosohr";
externalConnection.name = "Contoso HR";
externalConnection.description = "Connection to index Contoso HR system";

graphClient.external().connections()
    .buildRequest()
    .post(externalConnection);

```