---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d9e628e3a798e0d18f2143228612c5cc836fa96
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968426"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnniversary personAnniversary = new PersonAnniversary();
personAnniversary.allowedAudiences = EnumSet.of(AllowedAudiences.CONTACTS);

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .patch(personAnniversary);

```