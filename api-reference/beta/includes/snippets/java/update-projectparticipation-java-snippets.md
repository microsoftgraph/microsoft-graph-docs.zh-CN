---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5b82776c2edb5cb594ddf9427030be164a7cd3316d9eeb0fa93b71587a22e5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278370"
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