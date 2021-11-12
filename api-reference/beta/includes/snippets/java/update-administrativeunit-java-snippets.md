---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81f01ddf24fa226261f5176ce2f3175a31880843ebf16bae25e63c06d2354869
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104071"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "displayName-value";
administrativeUnit.description = "description-value";
administrativeUnit.visibility = "visibility-value";

graphClient.administrativeUnits("{id}")
    .buildRequest()
    .patch(administrativeUnit);

```