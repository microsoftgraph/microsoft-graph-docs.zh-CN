---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c9f08426adad888b75208aff9184df9adf15d978047de0f03f93b9c9e804b7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .GetAsync();

```