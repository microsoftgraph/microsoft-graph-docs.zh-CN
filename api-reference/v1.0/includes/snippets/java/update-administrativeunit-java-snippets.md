---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eabde6c1521f387d410fab775f20a665a2c5fc93
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Greater Seattle District Technical Schools";

graphClient.directory().administrativeUnits("4d7ea995-bc0f-45c0-8c3e-132e93bf95f8")
    .buildRequest()
    .patch(administrativeUnit);

```