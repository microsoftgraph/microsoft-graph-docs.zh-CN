---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e49ce56f00b8412c127a2fbd5f9d0f5f5f076e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775174"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
    .instantiate(displayName)
    .buildRequest()
    .post();

```