---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e23bbb41ebbe8b0450536308f7e0eb28d48c397
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920499"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2X_1_Partner").languages("en").overridesPages("selfasserted1_1").content()
    .buildRequest()
    .delete();

```