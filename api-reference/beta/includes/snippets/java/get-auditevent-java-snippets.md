---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e4c0ba36f55e1c72842335599060925244fbee1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393877"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content auditEvent = graphClient.tenantRelationships().managedTenants().auditEvent()
    .buildRequest()
    .get();

```