---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7a93375d46b8c68dfc625f915498f8959e327ac
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209315"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```