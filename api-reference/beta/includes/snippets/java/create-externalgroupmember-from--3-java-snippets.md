---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2ae9d094d234f26ec53533b4aa11a7c2cf054534b1375e7504f74a10e8481d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215889"
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