---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88b17cee095eed08a99c3a3c857b820c150dd659
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Teams["{id}"].Channels["{id}"].FilesFolder
    .Request()
    .GetAsync();

```