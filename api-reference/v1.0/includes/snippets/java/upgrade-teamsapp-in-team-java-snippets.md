---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94f0c7ef16752c0155f85b971ce186c8864f7e57
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690507"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("db5e04be-daa2-4a35-beb1-5e73cc381599").installedApps("NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=")
    .upgrade()
    .buildRequest()
    .post();

```