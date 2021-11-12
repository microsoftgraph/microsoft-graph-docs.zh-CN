---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81300fc7877a8cee888adb20d6a8bafde752d8f8fcaa01ada42656dea3691cea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

var password = "String";

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
    }
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,password,null,recipients)
    .Request()
    .PostAsync();

```