---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb529fa2d704245384c35f478dcbcb1e2dee9452
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = graphClient.devices("6a59ea83-02bd-468f-a40b-f2c3d1821983")
    .buildRequest()
    .select("id,extensionAttributes")
    .get();

```