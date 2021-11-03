---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab17d2cee1b4f28d944fb6d4e894f69359d4400920204fe9c8b4296235e90158
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns["{columnDefinition-id}"]
    .Request()
    .DeleteAsync();

```