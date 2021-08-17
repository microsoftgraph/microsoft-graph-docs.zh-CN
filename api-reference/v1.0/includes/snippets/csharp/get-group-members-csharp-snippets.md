---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c2cc06b953ed049816e19b1f2e9fd288d9e1b0a31634a1f6f9962fb43a7499
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{group-id}"].Members
    .Request()
    .GetAsync();

```