---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d09197c1b82d9e3ecdcc9e99987b76fe64d48cc0e0a3b18c7493f7bcd083c979
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview")
    .GetAsync();

```