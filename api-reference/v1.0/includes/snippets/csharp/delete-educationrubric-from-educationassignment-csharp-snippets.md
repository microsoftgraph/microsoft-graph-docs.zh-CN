---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39e14fb157816b5dcc7609e445e0229dd146c56f73d63ba6d0b10a675cb2e78d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric.Reference
    .Request()
    .DeleteAsync();

```