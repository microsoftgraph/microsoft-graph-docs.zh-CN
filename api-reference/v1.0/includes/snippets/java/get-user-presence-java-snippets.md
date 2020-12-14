---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74a5a9846fa4e07f2ca0c48a912ea15363c979cc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663944"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content presence = graphClient.users("66825e03-7ef5-42da-9069-724602c31f6b").presence()
    .buildRequest()
    .get();

```