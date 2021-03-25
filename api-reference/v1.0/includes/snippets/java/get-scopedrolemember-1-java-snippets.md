---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fb77a839011beb2c0976ecf145240d2ce82aaaa
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210743"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.directory().administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```