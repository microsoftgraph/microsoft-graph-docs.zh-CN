---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad4512e6b7e75b1d82be14e289f0d0d3dd742dcff0ecad6037d7dd3175f38b2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .DeleteAsync();

```