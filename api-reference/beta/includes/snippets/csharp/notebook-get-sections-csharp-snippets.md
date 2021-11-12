---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9dea2e2575fae368d44abe132b726e2be2cbd3bd6756baf946ca9054c1ddb61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Notebooks["{notebook-id}"].Sections
    .Request()
    .GetAsync();

```