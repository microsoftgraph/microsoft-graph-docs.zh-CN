---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df4c144300f8cbc55afbbff83a5f082c1e07fee1
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513647"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();
removeLicensesList.add(UUID.fromString("c7df2760-2c81-4ef7-b578-5b5392b571df"));
removeLicensesList.add(UUID.fromString("b05e124f-c7cc-45a0-a6aa-8cf78c946968"));

graphClient.groups("1132b215-826f-42a9-8cfe-1643d19d17fd")
    .assignLicense(GroupAssignLicenseParameterSet
        .newBuilder()
        .withAddLicenses(addLicensesList)
        .withRemoveLicenses(removeLicensesList)
        .build())
    .buildRequest()
    .post();

```