---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e192356023d16e1a51be12164df4f9c4f8f685563e332f99728dc8f77f4ba43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var relations = await graphClient.TermStore.Sets["{termStore.set-id}"].Relations
    .Request()
    .GetAsync();

```