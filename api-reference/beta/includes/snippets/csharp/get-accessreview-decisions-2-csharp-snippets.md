---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53e2c949385bb6ee464d8f1a78bf76a62f655c2d36725f563ed214b1c7563129
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myDecisions = await graphClient.AccessReviews["{accessReview-id}"].MyDecisions
    .Request()
    .GetAsync();

```