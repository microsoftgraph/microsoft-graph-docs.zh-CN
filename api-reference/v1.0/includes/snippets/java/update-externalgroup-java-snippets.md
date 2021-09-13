---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cb651053c468b39f133a87b7530b16164576ac8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022372"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = new ExternalGroup();
externalGroup.displayName = "Contoso Marketing";
externalGroup.description = "The product marketing team";

graphClient.connections("{connectionsId}").groups("{externalGroupId}")
    .buildRequest()
    .patch(externalGroup);

```