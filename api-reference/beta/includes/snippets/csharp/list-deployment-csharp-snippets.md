---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9fcacf657e54eccc63a4d1ad96c210798fc8950f89d6dcd7976bb92b72e849a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployments = await graphClient.Admin.Windows.Updates.Deployments
    .Request()
    .GetAsync();

```