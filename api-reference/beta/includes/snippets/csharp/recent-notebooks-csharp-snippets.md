---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f3f6fcbbb7137aa848e66b10e961c266eeaa75d93d7a614a094b7efdcb4dea9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getrecentnotebooks = await graphClient.Me.Onenote.Notebooks
    .Getrecentnotebooks(true)
    .Request()
    .GetAsync();

```