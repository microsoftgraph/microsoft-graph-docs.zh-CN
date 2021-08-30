---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8447814095f757c2ecbff73eefb7a4625e1bf4bb2bac0dfe06a65c4b0fb113b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161865"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroupMember externalGroupMember = new ExternalGroupMember();
externalGroupMember.id = "e5477431-1038-484e-bf69-1dfedb97a110";
externalGroupMember.type = ExternalGroupMemberType.GROUP;
externalGroupMember.identitySource = IdentitySourceType.AZURE_ACTIVE_DIRECTORY;

graphClient.external().connections("contosohr").groups("31bea3d537902000").members()
    .buildRequest()
    .post(externalGroupMember);

```