---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4de3ea61bab245265dfea8461f2411687c7edba0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963920"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Domain domain = new Domain();
domain.isDefault = true;
LinkedList<String> supportedServicesList = new LinkedList<String>();
supportedServicesList.add("Email");
supportedServicesList.add("OfficeCommunicationsOnline");
domain.supportedServices = supportedServicesList;

graphClient.domains("contoso.com")
    .buildRequest()
    .patch(domain);

```