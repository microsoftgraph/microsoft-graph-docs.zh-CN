---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf2ca72f6d755b702876e7b28d9dbc0ae6ba788bfcfc77102ebea30d54bb1860
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Events["{event-id}"]
    .Request()
    .DeleteAsync();

```