---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 852698a29ae41d888efbed053deeaea0bedc1c59693e82447256f8ed7594af76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{notebook-id}"]
    .Request()
    .GetAsync();

```