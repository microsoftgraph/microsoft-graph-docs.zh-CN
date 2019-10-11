---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8af8695e1f2b9e227f639b4a8ed64937ac4cd34
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"].Content
    .Request()
    .GetAsync();

```