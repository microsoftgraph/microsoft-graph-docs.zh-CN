---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a54359ba0aee0f1f6bd7e30b04c7c259a876603bb5b8dcdd4daf5d888c5ce7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .get();

```