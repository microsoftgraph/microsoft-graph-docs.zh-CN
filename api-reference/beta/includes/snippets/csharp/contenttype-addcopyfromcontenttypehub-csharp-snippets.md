---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c5bc7348d93a985333ca54cb36541b00a3e45d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypeId = "String";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopyFromContentTypeHub(contentTypeId)
    .Request()
    .PostAsync();

```