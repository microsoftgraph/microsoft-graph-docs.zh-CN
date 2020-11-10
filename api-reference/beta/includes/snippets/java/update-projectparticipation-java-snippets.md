---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3b6380c8d5bd02f753d63c295de1e5cb3c0dd2e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968954"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = new ProjectParticipation();
projectParticipation.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);
CompanyDetail client = new CompanyDetail();
client.department = "Corporate Marketing";
client.webUrl = "https://www.contoso.com";
projectParticipation.client = client;

graphClient.me().profile().projects("{id}")
    .buildRequest()
    .patch(projectParticipation);

```