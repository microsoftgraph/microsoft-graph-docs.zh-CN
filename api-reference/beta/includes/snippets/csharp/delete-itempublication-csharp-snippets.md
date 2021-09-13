---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d42944c8c704c83eb5f02ffae4b3fff1cbf0d07fa0bef0bc720b15bb458bd0e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Publications["{itemPublication-id}"]
    .Request()
    .DeleteAsync();

```