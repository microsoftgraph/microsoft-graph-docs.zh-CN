---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c7208a34ca24c19382814d51d497d9ca82162d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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