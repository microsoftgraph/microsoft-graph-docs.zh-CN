---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d730b87056c42b8f806b75c7d0adaf42dcc50471321ea3a71b5b52ee2fb91ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimesOff["{timeOff-id}"]
    .Request()
    .DeleteAsync();

```