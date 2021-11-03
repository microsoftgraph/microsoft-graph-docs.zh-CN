---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c195d8657396f045f187cd2789c927a3b052d72
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = await graphClient.External.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .GetAsync();

```