---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 561e704dfae1a5344e9be64a6446c5580e71440d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314206"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("root").lists("Documents")
    .buildRequest()
    .get();

```