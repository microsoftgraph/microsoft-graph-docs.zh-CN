---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97d3fc6f49e553922b9b4feca423e5539070fd6492f8c8248acca659438508d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Request()
    .GetAsync();

```