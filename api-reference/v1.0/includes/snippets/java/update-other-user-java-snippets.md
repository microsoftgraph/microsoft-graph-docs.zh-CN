---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f76e9d6e6872733ab10078f3c44a7f623ad229e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 425 555 0109");
user.businessPhones = businessPhonesList;
user.officeLocation = "18/2111";

graphClient.users("{id}")
    .buildRequest()
    .patch(user);

```