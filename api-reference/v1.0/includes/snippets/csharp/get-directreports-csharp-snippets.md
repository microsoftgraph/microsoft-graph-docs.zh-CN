---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3b6f1e15cf785b5fb57bfbc1e57983fb68df58e66b0eeaba3b78993a2863554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Me.DirectReports
    .Request()
    .GetAsync();

```