---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d2350a055bff41a4046332a042a95c0b34e558fc21e786ad253f8594ac9cd01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .GetAsync();

```