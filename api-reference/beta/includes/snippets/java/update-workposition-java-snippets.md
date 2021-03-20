---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1baddf69c997f150be0bb98fa311d5557f67b4e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = new WorkPosition();
workPosition.isCurrent = true;

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .patch(workPosition);

```