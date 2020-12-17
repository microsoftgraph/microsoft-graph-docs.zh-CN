---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f945cff9a5d7c0b3d7346169a0e1d6ef2cf8f09
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692730"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("{id}")
    .buildRequest()
    .get();

```