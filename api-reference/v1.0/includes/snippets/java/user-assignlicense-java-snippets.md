---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8050440dfd67043bbbdd7a17f696736577c14e98
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886935"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();
AssignedLicense addLicenses = new AssignedLicense();
LinkedList<String> disabledPlansList = new LinkedList<String>();
disabledPlansList.add("11b0131d-43c8-4bbb-b2c8-e80f9a50834a");
addLicenses.disabledPlans = disabledPlansList;
addLicenses.skuId = "guid";

addLicensesList.add(addLicenses);

LinkedList<String> removeLicensesList = new LinkedList<String>();
removeLicensesList.add("bea13e0c-3828-4daa-a392-28af7ff61a0f");

graphClient.me()
    .assignLicense(addLicensesList,removeLicensesList)
    .buildRequest()
    .post();

```