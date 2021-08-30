---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 036195ae36d8f77a2346ad7f710ba741e82e80b5b8a0ab30b5ba42c4265f3d55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161870"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "e811976d-83df-4cbd-8b9b-5215b18aa874";
externalGroupMember.type = ExternalGroupMemberType.USER;
externalGroupMember.identitySource = IdentitySourceType.AZURE_ACTIVE_DIRECTORY;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```