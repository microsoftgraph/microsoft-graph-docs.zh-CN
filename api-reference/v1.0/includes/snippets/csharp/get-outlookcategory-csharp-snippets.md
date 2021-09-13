---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 332f29908a5dd0abd5b947a3812cbfd2831ca4bf7fc26ab226f0ea6989fe1c8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = await graphClient.Me.Outlook.MasterCategories["{outlookCategory-id}"]
    .Request()
    .GetAsync();

```