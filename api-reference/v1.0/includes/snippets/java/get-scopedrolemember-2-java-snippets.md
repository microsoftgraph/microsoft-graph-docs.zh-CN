---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a527b0f73b8bc5c1e2edbe8118d5ce44eb781c4bf2d3fad22696cb4a342d6ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333161"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.directory().administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```