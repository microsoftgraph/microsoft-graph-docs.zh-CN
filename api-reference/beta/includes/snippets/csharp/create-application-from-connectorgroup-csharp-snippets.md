---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 617f1416744431ee78d24373c18cc1a95b4d6276aab2a18679b3179bfcf2b365
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ConnectorGroup.Reference
    .Request()
    .PutAsync("{id}");

```