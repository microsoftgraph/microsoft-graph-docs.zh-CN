---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f8033eb24344a6e9f121bebb84043936b246db
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691204"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["acda442c-78d2-491b-8204-4ef5019c0193"].InstalledApps
    .Request()
    .Filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .Expand("teamsAppDefinition")
    .GetAsync();

```