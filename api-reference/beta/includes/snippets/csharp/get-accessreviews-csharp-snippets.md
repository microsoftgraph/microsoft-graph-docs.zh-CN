---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 134c6473f33e7578d82229d32ac2f401476f12c1
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38710286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviews = await graphClient.AccessReviews
    .Request()
    .Filter("businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .GetAsync();

```