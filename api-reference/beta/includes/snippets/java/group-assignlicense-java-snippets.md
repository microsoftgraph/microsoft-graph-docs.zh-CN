---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c418efa9bca17a8390a017e822e861d345282aa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980815"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();
AssignedLicense addLicenses = new AssignedLicense();
LinkedList<UUID> disabledPlansList = new LinkedList<UUID>();
disabledPlansList.add(UUID.fromString("11b0131d-43c8-4bbb-b2c8-e80f9a50834a"));
addLicenses.disabledPlans = disabledPlansList;
addLicenses.skuId = UUID.fromString("skuId-value-1");

addLicensesList.add(addLicenses);
AssignedLicense addLicenses1 = new AssignedLicense();
LinkedList<UUID> disabledPlansList1 = new LinkedList<UUID>();
disabledPlansList1.add(UUID.fromString("a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235"));
addLicenses1.disabledPlans = disabledPlansList1;
addLicenses1.skuId = UUID.fromString("skuId-value-2");

addLicensesList.add(addLicenses1);

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();

graphClient.groups("1ad75eeb-7e5a-4367-a493-9214d90d54d0")
    .assignLicense(GroupAssignLicenseParameterSet
        .newBuilder()
        .withAddLicenses(addLicensesList)
        .withRemoveLicenses(removeLicensesList)
        .build())
    .buildRequest()
    .post();

```