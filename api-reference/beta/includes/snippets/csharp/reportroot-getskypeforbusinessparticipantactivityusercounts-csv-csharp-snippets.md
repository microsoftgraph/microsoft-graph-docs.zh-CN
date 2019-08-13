---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6872cb8a15ddb364bf4cedc489c44fba4603fd40
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityUserCounts("D7")
    .Request()
    .GetAsync();

```