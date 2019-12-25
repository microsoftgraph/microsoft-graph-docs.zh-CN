---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9711b78ea4109d6d564f935aa924277f684b892
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Users["66825e03-7ef5-42da-9069-724602c31f6b"].Presence
    .Request()
    .GetAsync();

```