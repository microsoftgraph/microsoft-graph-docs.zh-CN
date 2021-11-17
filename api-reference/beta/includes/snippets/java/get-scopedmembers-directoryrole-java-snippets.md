---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e90e8cc73cdfad03de3ff64255144de9563e63454f9d06e71439b976dfd1044
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332731"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedMembers = graphClient.directoryRoles("41d12a2f-caa8-4e3e-ba14-05e5102ce085").scopedMembers()
    .buildRequest()
    .get();

```