---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d322a567c0a56dbdb54c0f91dbfc616dd12ff5642763f51def26b91b0be5567
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["{group-id}"].Events["{event-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```