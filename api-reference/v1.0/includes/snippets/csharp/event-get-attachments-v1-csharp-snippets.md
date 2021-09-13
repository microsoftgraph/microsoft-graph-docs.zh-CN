---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b5f42e7f5452f0c00063ff99fccdaf261d76322df6c5ef15e0caabd0be2b244
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Events["{event-id}"].Attachments
    .Request()
    .GetAsync();

```