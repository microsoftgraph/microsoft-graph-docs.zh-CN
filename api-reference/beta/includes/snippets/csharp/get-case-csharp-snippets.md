---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4164479e4cc07f8f25e31a52909169ec757eee328198730b00052382e951d7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .GetAsync();

```