---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6c6c495225198c7e8e0fe9cc92bea1f06953f75
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223629"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "HiddenMembership";

graphClient.directory().administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```