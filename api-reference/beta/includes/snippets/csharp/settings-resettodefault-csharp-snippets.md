---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 885fcaf8f238a7c78150b2b7e2934285889d1ca9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Settings
    .Resettodefault()
    .Request()
    .PostAsync();

```