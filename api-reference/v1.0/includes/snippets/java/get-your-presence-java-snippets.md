---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 025f958afc325612c85fffe1f5fdba1b10f7b864
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690545"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.me().presence()
    .buildRequest()
    .get();

```