---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e97dba362dd99ad61696f24c1e9646d914e6a6315b188e3cfaecdca05e70a81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .DeleteAsync();

```