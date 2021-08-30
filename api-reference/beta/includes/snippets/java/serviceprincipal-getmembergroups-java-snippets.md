---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29f77139a160394a6158b3123480f5dbb8994ec4b9c41b2b90dbd0bfcd2fbed7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.servicePrincipals("{id}")
    .getMemberGroups(DirectoryObjectGetMemberGroupsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```