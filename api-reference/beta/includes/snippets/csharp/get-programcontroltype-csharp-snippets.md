---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17aefe397f4ecc01a5f2fbd8264bf6854f09d391dc3fa747f8e4c32282b4118e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControlTypes = await graphClient.ProgramControlTypes
    .Request()
    .GetAsync();

```