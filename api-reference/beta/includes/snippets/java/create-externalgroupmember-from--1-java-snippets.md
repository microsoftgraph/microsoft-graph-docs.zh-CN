---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 933facb989f64489c6e305d57b5345a9e0b9c764
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209937"
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