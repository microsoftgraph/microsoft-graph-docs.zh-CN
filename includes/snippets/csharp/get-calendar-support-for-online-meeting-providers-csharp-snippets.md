---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc213b85640e68225f6342057a24ee656789b2fec0df8acbe5975cc2ec62917
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Me.Calendar
    .Request()
    .GetAsync();

```