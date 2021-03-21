---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04b7db5b3f2e2ea29e6a8ee484a124c6e41f6c1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974129"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = graphClient.print().taskDefinitions("3203656e-6069-4e10-8147-d25290b00a3c").tasks("d036638b-1272-4bba-9227-732463823ed3")
    .buildRequest()
    .get();

```