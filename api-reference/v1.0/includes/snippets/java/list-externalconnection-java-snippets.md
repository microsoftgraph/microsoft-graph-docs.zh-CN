---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca667843f3b86270996b2e6b2c8b6b2f12786013
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnectionCollectionPage connections = graphClient.connections()
    .buildRequest()
    .get();

```