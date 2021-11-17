---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ba0026c32c29e1ba35561ab5e5f1859661e695658d9f06fe91f418d3de2b36f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .DeleteAsync();

```