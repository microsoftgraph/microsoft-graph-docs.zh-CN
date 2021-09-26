---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d591359fdc119e8f7ce7e1846935e9b38af2a089418f1e6533594df20cefea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277435"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Contoso Life v2.0";
group.displayName = "Contoso Life Renewed";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```