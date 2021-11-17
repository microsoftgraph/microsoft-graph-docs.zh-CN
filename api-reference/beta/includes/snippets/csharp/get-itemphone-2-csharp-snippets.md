---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 751c60c8ce9e8fc5ace38b39ca8b357437ffe16f2118def25d3fa2b9ed0f775a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phones = await graphClient.Me.Profile.Phones
    .Request()
    .GetAsync();

```