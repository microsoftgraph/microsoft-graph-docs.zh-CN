---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2e83054aebaeb6d179c5b411eab53e241c42c15
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = await graphClient.Me.Profile.Languages["{id}"]
    .Request()
    .GetAsync();

```