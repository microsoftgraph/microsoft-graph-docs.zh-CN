---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eed34c02a38a43312fce1c8623832cb006fbdcb930cbd5f6cd96fe68c815c8f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "displayName-value";
administrativeUnit.description = "description-value";
administrativeUnit.visibility = "visibility-value";

graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .patch(administrativeUnit);

```