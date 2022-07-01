---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5b2d0e851ba755c478187bf25e7997037d17cf
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppUserDetail("D7")
    .Request()
    .GetAsync();

```