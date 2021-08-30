---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55e7c40543a37f0e165449f7143ea0f7d849f55da281b870fbc1f97c0a4bbf16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Members
    .Request()
    .GetAsync();

```