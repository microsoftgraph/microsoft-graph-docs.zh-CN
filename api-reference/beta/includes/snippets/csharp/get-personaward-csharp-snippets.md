---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 446eb86ac910df5d57fc52bd9d5c748467acbd8974c9eca3b4e8c8cf6743f491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = await graphClient.Me.Profile.Awards["{personAward-id}"]
    .Request()
    .GetAsync();

```