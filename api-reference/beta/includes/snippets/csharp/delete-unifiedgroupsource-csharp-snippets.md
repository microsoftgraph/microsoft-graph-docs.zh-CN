---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08ce87fcf035b2ce68395e4180a10f702e5671b8
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscoveryCaseId}"].Custodians["{custodianId}"].UnifiedGroupSources["{unifiedGroupSourceId}"]
    .Request()
    .DeleteAsync();

```