---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3ac0b46dcceb09cdd8608807d98338c4f20c81e1f0a37a470a2c230d38ca91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220714"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinition columnDefinition = new ColumnDefinition();
columnDefinition.required = true;
columnDefinition.hidden = false;
columnDefinition.propagateChanges = false;

graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns("{column-id}")
    .buildRequest()
    .patch(columnDefinition);

```