---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e28bf999ad98c2fcd5d04f9dc791906878d27dd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975037"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("businessPhones-value");
user.businessPhones = businessPhonesList;
user.officeLocation = "city-value";

graphClient.users("{id}")
    .buildRequest()
    .patch(user);

```