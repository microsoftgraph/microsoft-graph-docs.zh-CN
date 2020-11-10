---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3a6b960e9a8e2e055f2d27a3ee90dca9ed42802
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();
removeLicensesList.add(UUID.fromString("skuId-value-1"));
removeLicensesList.add(UUID.fromString("skuId-value-2"));

graphClient.groups("1ad75eeb-7e5a-4367-a493-9214d90d54d0")
    .assignLicense(addLicensesList,removeLicensesList)
    .buildRequest()
    .post();

```