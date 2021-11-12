---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e27205ce110aab8e7c6eec7da0355c70eab37c4b4c4c5a9dcb2a89045526bbe2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Print.Shares
    .Request()
    .GetAsync();

```