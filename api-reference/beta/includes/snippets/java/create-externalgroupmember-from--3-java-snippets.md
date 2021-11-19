---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcd857cc37ec417789830f7535c443625ed05f03
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "1431b9c38ee647f6a";
externalGroupMember.type = ExternalGroupMemberType.USER;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```