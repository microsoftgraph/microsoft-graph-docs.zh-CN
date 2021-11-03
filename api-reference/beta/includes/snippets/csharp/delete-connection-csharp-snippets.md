---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ba66bf52086c772b367b8b8b02cfc0ede71d8be
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .DeleteAsync();

```