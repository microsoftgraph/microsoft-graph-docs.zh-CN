---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec64c6a00ba321cd89ee46f9ea5041582d432d4abde76290fa284cd13e7f77a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var thumbnails = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails
    .Request()
    .GetAsync();

```