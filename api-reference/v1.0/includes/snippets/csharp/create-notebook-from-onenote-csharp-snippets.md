---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 756ff7e43e59ca811f93b0e675aa8250c1e88dfb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = new Notebook
{
    DisplayName = "My Private notebook"
};

await graphClient.Me.Onenote.Notebooks
    .Request()
    .AddAsync(notebook);

```