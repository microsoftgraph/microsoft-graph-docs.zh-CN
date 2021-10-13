---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a750d051aa1473876f93518a5a5dec0bc55cf0bd0fca1301e310e8e896696dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredOwners = await graphClient.Devices["{device-id}"].RegisteredOwners
    .Request()
    .GetAsync();

```