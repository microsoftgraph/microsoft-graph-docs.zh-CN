---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6625b720f63c7da81271ca85e2ee309e40c0024e9ba3055e6a48e4320451079b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Programs["{program-id}"]
    .Request()
    .DeleteAsync();

```