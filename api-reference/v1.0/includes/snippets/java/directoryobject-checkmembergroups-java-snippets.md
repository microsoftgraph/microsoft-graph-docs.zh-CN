---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5f2cbbe1558abcf2ce1cd09d73db1b71517c63e8ce1c6401a044c5e1c6b3a2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903360"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64b130f4eb9e75525e");
groupIdsList.add("4fe90ae065a-478b9400e0a0e1cbd540");

graphClient.directoryObjects("{id}")
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```