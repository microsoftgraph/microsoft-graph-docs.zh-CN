---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 030ab885b4c201cd967d7b098457b25e627c7b6e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b"
};

await graphClient.Communications
    .GetPresencesByUserId(ids)
    .Request()
    .PostAsync();

```