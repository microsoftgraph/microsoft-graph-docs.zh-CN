---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be619a3c566291957fb54c2076d51166bde764150b8dcdc4582de20d9450863a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902566"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```