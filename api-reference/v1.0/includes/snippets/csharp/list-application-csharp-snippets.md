---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8ec430847547401ea293a5e8a3512401a4af0f97cba4743f2f6cd8a1dd61976
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .GetAsync();

```