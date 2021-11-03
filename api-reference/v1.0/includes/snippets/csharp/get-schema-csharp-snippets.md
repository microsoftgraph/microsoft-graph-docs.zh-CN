---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c028fafa438b718439dbffd89cc31c0fbb2ce6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Schema
    .Request()
    .GetAsync();

```