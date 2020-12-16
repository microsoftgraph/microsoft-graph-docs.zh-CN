---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cfdfe991a38ef04083dcfb8db1f79cf4dea8a83
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690547"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.users("66825e03-7ef5-42da-9069-724602c31f6b").presence()
    .buildRequest()
    .get();

```