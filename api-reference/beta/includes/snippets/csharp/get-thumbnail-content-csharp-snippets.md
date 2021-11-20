---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adfa45220ecfcff0b737460c6b5aade86162f143a88f9f74221cc7ba283bdc6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails["{thumbnailSet-id}"]["{thumbnailSet-id}"].Content
    .Request()
    .GetAsync();

```