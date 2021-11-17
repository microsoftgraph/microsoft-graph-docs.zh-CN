---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7d8eb6b83e3afae96d8c2368903582660d68fb8e3d24baf76b07c70b8a553cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var interests = await graphClient.Me.Profile.Interests
    .Request()
    .GetAsync();

```