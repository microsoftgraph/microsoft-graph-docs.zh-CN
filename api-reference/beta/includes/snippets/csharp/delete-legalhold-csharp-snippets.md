---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c668ec878fdac352945f95c21ec56b659e0b23d070a60856c5a6c19408250bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"]
    .Request()
    .DeleteAsync();

```