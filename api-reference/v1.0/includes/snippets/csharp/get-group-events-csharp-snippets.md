---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e86a84c401346fc035ee44adf2fbb0cbc6b83f3d2bd307a16c1ad0d10a078ebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107040"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["{group-id}"].Events
    .Request()
    .GetAsync();

```