---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c6f28004243a67193a85f060ac8af76b6925d52
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Admin.ServiceAnnouncement.Messages["{serviceUpdateMessage-id}"].Attachments["{serviceAnnouncementAttachment-id}"].Content
    .Request()
    .GetAsync();

```