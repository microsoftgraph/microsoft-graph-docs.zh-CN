---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee32be76a31b369cc2ff1c261b580a70c12ad69b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Filter("contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')")
    .GetAsync();

```