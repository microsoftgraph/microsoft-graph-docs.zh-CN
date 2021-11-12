---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de03e143429a94a151b58ad7b218cfe300a6395ab07fdc824e4b299b2e0b2862
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Education.Classes["{educationClass-id}"].Group
    .Request()
    .GetAsync();

```