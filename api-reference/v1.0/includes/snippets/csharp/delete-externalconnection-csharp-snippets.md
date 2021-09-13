---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc19af6e26d82e6b0c860148bb3db5c62ee60da0228856548d43e88ed74e4691
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .DeleteAsync();

```