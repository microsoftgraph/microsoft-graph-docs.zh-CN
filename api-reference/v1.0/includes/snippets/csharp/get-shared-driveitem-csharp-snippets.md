---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b5dfd0404dce0dc61251b350fef13bd4d4c539e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{shareIdOrUrl}"].DriveItem
    .Request()
    .GetAsync();

```