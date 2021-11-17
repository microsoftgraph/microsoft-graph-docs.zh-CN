---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02231e9df6bfc2f7fa069c3333144b0f11a5f7ff5f545d8b23b7fac9090ac142
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var asHierarchy = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags
    .AsHierarchy()
    .Request()
    .GetAsync();

```