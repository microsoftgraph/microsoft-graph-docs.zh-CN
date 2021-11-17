---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93881cc38b6fcc96d55e6c6447cdd2d3acf8e47f55ae95966a8c20e078bdedbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroups = await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups
    .Request()
    .GetAsync();

```