---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64d3de1c4156d7882374582fd2ad346e35e42687f84d4b47d6efb3b5111ac68f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScore = await graphClient.Security.SecureScores["{secureScore-id}"]
    .Request()
    .GetAsync();

```