---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d00cd8e2d980c3c77cf56b76d56dd0b4d5e0aeb0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "e5477431-1038-484e-bf69-1dfedb97a110";
externalGroupMember.type = ExternalGroupMemberType.USER;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```