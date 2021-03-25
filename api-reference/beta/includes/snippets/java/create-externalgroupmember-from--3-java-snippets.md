---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adf6a27fd39bfa0e6301d8ac1534490a58ab5d42
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "1431b9c38ee647f6a";
externalGroupMember.type = ExternalGroupMemberType.GROUP;
externalGroupMember.identitySource = IdentitySourceType.EXTERNAL;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```