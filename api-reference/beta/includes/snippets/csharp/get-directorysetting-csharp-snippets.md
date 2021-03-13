---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fc4bd0bb7140027451b928ab49fd170b30ebfad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = await graphClient.Settings["{directorySetting-id}"]
    .Request()
    .GetAsync();

```