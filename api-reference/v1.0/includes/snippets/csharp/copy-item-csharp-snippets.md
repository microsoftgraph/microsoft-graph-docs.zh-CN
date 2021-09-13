---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5fece91a3b00c0cda819ac437126a12ea2973ef81c8a31c75343173685d00e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    DriveId = "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    Id = "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
};

var name = "contoso plan (copy).txt";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Copy(name,parentReference)
    .Request()
    .PostAsync();

```