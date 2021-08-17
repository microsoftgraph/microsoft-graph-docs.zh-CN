---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ef6213198201205be3b29bb992ec25089f773dbf1f2fe0124152fff880f03a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .GetAsync();

```