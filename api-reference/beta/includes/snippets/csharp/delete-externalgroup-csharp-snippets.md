---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a043cba5afc069da8b6f1f59ad7109cfc0361fac06c6413f35dd91398d5adacb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"]
    .Request()
    .DeleteAsync();

```