---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afee50aba86a3cc5696131fbd5b3ad84c3c6893f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525544"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content lists = graphClient.me().tasks().lists()
    .buildRequest()
    .get();

```