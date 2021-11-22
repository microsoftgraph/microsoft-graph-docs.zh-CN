---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d75d7d6a070d0e4d29d17ae04191da1004525b55c5c483e3b12274e5a4080899
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programs = await graphClient.Programs
    .Request()
    .GetAsync();

```