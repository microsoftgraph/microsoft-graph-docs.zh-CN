---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec844418b8ab30ce428094bd0b9ce626400298de3661ab4d241cbda303272fe1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = new OnenoteSection
{
    DisplayName = "Section name"
};

await graphClient.Me.Onenote.Notebooks["{notebook-id}"].Sections
    .Request()
    .AddAsync(onenoteSection);

```