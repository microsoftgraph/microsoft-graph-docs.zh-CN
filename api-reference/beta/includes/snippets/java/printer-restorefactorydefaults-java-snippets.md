---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4873f733022cb3c0a8b7b2d847a5201273cb901
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970291"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```