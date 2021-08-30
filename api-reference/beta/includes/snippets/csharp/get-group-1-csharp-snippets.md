---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 049577178212003b242c04725a62f8d5bd2358e9c4b7bce9be3d2b2fa8c3ca44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"]
    .Request()
    .GetAsync();

```