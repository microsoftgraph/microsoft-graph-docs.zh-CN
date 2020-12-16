---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47ff81bad394fc2e68ce7481e805d5f6dc0cf299
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["db5e04be-daa2-4a35-beb1-5e73cc381599"].InstalledApps["NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg="]
    .Upgrade()
    .Request()
    .PostAsync();

```