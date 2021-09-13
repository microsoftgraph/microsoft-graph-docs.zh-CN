---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 156f7ff0b182b8698147eb4e12eb6c35e06c119b5dbbdf2cd4479bbc271b5691
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Tasks
    .Request()
    .GetAsync();

```