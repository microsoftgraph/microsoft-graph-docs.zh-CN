---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f93ebfc3c12d0b88fa77b53fe1eeeee2a94a3191
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```