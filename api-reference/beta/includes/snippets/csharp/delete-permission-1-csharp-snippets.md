---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b959f0d6e3f4b46c7d30f9432a4d8f41d8a8883c42da075630b6f02caaabba47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .Request()
    .DeleteAsync();

```