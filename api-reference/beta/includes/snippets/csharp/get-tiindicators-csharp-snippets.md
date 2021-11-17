---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7b8e89679f9d328253ddb3f0b4d1b58b76cca82113ed107bae5bd00f63e3a3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218440"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicators = await graphClient.Security.TiIndicators
    .Request()
    .GetAsync();

```