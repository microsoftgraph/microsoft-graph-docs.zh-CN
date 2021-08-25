---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d34bbb7396b9d1866732c73fea1d797e10defe23c14e077e29f4dd5cc534d8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = await graphClient.Settings["{directorySetting-id}"]
    .Request()
    .GetAsync();

```