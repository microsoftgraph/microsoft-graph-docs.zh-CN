---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 934d3e21d9a3ae097250643e3d3cc92b55305399
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();
AssignedLicense addLicenses = new AssignedLicense();
LinkedList<UUID> disabledPlansList = new LinkedList<UUID>();
disabledPlansList.add(UUID.fromString("8a256a2b-b617-496d-b51b-e76466e88db0"));
addLicenses.disabledPlans = disabledPlansList;
addLicenses.skuId = UUID.fromString("84a661c4-e949-4bd2-a560-ed7766fcaf2b");

addLicensesList.add(addLicenses);
AssignedLicense addLicenses1 = new AssignedLicense();
LinkedList<UUID> disabledPlansList1 = new LinkedList<UUID>();
addLicenses1.disabledPlans = disabledPlansList1;
addLicenses1.skuId = UUID.fromString("f30db892-07e9-47e9-837c-80727f46fd3d");

addLicensesList.add(addLicenses1);

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();

graphClient.me()
    .assignLicense(UserAssignLicenseParameterSet
        .newBuilder()
        .withAddLicenses(addLicensesList)
        .withRemoveLicenses(removeLicensesList)
        .build())
    .buildRequest()
    .post();

```