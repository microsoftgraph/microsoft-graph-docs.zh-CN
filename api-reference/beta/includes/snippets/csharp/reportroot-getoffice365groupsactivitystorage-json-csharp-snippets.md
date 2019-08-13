---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e46a6ff6125d7901f4c4ca657808362331440bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityStorage = await graphClient.Reports
    .GetOffice365GroupsActivityStorage("D7")
    .Request()
    .GetAsync();

```