---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c22e0a700fc826123b21e8b60501f57268e72a31
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210592"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "description-value";
group.displayName = "displayName-value";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```