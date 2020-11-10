---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e01d044280c61aed95973ae845d9e47527a92af
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970890"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.servicePrincipals("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```