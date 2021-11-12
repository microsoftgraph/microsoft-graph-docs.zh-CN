---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb3db4ef13e0a795a7a5b9dd522f8dc37d905b677908dcdd1c83ad2c476402ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```