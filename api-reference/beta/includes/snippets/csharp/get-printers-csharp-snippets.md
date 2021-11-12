---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa4a395e0831a1101b005ca44b857b4a7a2719b9398e23d04ce49596d68ec417
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printers = await graphClient.Print.Printers
    .Request()
    .GetAsync();

```