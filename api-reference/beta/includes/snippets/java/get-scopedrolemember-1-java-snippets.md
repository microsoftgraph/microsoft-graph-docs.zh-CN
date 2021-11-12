---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c6d4b822cc9569ea607da878573fee11b3fa790b3949339a751915bbb4020b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```