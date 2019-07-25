---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d5e764062252be4b783ce8486ece223273fd6d0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedLanguages = await graphClient.Me.Outlook
    .SupportedLanguages()
    .Request()
    .GetAsync();

```