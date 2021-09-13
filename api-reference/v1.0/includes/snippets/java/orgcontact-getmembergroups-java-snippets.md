---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 976a13a3769b56999d7d9e09ac2fa022c04fdc580760cbc38f4180bc795af8e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.contacts("{id}")
    .getMemberGroups(DirectoryObjectGetMemberGroupsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```