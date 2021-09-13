---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6ee3e2e4c929e4a593493b09e405da1dd4e1c1d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Identity identity = new Identity();
identity.id = "e811976d-83df-4cbd-8b9b-5215b18aa874";
identity.type = IdentityType.USER;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(identity);

```