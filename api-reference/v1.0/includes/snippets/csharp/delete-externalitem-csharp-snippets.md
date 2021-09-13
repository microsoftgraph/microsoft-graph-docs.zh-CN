---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0a45776b9951eb7b763670887c6c87169b0a443660bfe8c51be4241ed6e7a2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .DeleteAsync();

```