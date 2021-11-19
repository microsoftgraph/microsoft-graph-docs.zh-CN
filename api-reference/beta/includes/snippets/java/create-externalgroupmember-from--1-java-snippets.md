---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a780517321414abe7d6c73b9c424d834e1c1afe1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102635"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "e811976d-83df-4cbd-8b9b-5215b18aa874";
externalGroupMember.type = ExternalGroupMemberType.USER;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```