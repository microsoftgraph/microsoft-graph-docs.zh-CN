---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4427aa746ef4d5844fc2f0ec0c12cd452954838a5be26cf179e8578817ccf875
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.Connections["{externalConnectors.externalConnection-id}"].Schema
    .Request()
    .GetAsync();

```