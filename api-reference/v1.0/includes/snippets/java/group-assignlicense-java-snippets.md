---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e80fcc3ae3e13f8f3009fbf2926da29135ff4f5a
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953668"
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

graphClient.groups("1ad75eeb-7e5a-4367-a493-9214d90d54d0")
    .assignLicense(addLicensesList,removeLicensesList)
    .buildRequest()
    .post();

```