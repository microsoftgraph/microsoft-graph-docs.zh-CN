---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd218df5901a58acdbae4701e00903eb14be2459
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867908"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();
AssignedLicense addLicenses = new AssignedLicense();
LinkedList<String> disabledPlansList = new LinkedList<String>();
disabledPlansList.add("11b0131d-43c8-4bbb-b2c8-e80f9a50834a");
addLicenses.disabledPlans = disabledPlansList;
addLicenses.skuId = "skuId-value-1";

addLicensesList.add(addLicenses);
AssignedLicense addLicenses1 = new AssignedLicense();
LinkedList<String> disabledPlansList = new LinkedList<String>();
disabledPlansList.add("a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235");
addLicenses1.disabledPlans = disabledPlansList1;
addLicenses1.skuId = "skuId-value-2";

addLicensesList.add(addLicenses1);

LinkedList<String> removeLicensesList = new LinkedList<String>();

graphClient.me()
    .assignLicense(addLicensesList,removeLicensesList)
    .buildRequest()
    .post();

```