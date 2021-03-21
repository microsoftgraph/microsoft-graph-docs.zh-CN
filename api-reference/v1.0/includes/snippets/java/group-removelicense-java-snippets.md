---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4edb00e13b2e3816aa94d71884767a3def9eb075
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966524"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();
removeLicensesList.add(UUID.fromString("skuId-value-1"));
removeLicensesList.add(UUID.fromString("skuId-value-2"));

graphClient.groups("1ad75eeb-7e5a-4367-a493-9214d90d54d0")
    .assignLicense(GroupAssignLicenseParameterSet
        .newBuilder()
        .withAddLicenses(addLicensesList)
        .withRemoveLicenses(removeLicensesList)
        .build())
    .buildRequest()
    .post();

```