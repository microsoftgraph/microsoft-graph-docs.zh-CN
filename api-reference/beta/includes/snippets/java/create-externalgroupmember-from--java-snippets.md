---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbaead62594f8ad7f790588583255a3bbb65f8bd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954627"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "1431b9c38ee647f6a";
externalGroupMember.type = ExternalGroupMemberType.GROUP;
externalGroupMember.identitySource = IdentitySourceType.EXTERNAL;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```