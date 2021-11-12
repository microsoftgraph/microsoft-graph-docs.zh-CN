---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3578b65ed1bdefe2c29123618279d2fa345cda890504318d00dbe6e105fec58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .Request()
    .GetAsync();

```