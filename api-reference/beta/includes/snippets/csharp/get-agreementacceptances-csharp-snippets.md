---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f151b8dbc27407d5af305545cdec9888b79bee8a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementAcceptances = await graphClient.Me.AgreementAcceptances
    .Request()
    .GetAsync();

```