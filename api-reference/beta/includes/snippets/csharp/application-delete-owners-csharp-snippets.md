---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88a91fa85f53245d8bf3738166a5856fc9a0be0cd239897ff5d233889075bc87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].Owners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```