---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1ecaddd99b3127ca2ee3ce6a0d565c15c1e3b2d567cf390762d255ff44fecb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219650"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Schools
    .Request()
    .GetAsync();

```