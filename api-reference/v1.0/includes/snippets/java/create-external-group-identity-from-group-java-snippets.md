---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f22766a7ea448a6889747db2bacaf3b20430df9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Identity identity = new Identity();
identity.id = "1431b9c38ee647f6a";
identity.type = IdentityType.EXTERNAL_GROUP;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(identity);

```