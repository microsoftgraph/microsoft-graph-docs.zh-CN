---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e148aebdbe1bedf9e5515d18ad52c7d885791994b001778191c2d4f3f25ef4ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104415"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64-b130-f4eb9e75525e");
groupIdsList.add("4fe90ae7-065a-478b-9400-e0a0e1cbd540");

graphClient.me()
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```