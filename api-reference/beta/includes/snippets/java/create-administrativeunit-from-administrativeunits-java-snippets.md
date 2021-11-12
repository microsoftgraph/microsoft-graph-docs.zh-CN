---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84a80e72b3d10bc61e2a1274be359f5f0b5580526610b0a0bb431242a383b871
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104079"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "HiddenMembership";

graphClient.administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```