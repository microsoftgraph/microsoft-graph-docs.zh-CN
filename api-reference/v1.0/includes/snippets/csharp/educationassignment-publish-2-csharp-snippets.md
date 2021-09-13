---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb890cda496484523201a32203f7cf3f88898b7d609b0c016af7ccce9aea9160
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Publish()
    .Request()
    .PostAsync();

```