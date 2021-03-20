---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cd86acc410930b54255405a4ebec5ab77ec8f68
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944229"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "description-value";
group.displayName = "displayName-value";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```