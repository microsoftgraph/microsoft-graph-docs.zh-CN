---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8a23858e656c970a06fdc749df1e3da05eef6ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945537"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.directory().administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```