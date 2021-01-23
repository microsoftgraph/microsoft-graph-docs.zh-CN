---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48294f8d24745301bb470858afc2b63333ae08ce
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directoryObject", "{}"}
    }
};

await graphClient.Contacts["{id}"].DirectReports
    .Request()
    .AddAsync(directoryObject);

```