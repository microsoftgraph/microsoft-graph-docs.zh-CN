---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cbe8a27ed3536ba92143571192b4b599626a3ba
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MyRoleCollectionPage myRoles = graphClient.tenantRelationships().managedTenants().myRoles()
    .buildRequest()
    .get();

```