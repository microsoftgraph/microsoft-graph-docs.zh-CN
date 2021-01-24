---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f721630ca04c623840eb37a8ee1d0a66adf1b4ef
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945622"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.directory().administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```