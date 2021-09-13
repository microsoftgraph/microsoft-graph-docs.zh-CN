---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93b42f9890d962ded325b39680776d1d749015d23e9d54cba5775ba33db52a51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webUrl = "webUrl value";

await graphClient.Me.Onenote.Notebooks
    .GetNotebookFromWebUrl(webUrl)
    .Request()
    .PostAsync();

```