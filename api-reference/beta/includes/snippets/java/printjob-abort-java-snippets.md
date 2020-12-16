---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a2349d78e02ffca8dd11e5d0448ca626f607ea9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691047"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}").jobs("{id}")
    .abort(null)
    .buildRequest()
    .post();

```