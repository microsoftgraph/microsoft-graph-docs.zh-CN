---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e49ce56f00b8412c127a2fbd5f9d0f5f5f076e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
    .instantiate(displayName)
    .buildRequest()
    .post();

```