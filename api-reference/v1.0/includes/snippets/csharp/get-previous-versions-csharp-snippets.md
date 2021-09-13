---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d2900f01a90867ad63ded2a0e75eb90f65b4655e12d2f72a419f051ca27896a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions
    .Request()
    .GetAsync();

```