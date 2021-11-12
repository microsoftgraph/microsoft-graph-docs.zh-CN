---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3ff1464f01f12e7db4611a037dbecfe4ef4ae060b75e9c7b1d91205d8f6a51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = new Microsoft.Graph.Ediscovery.Tag
{
    Description = "This is an updated description."
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"]
    .Request()
    .UpdateAsync(tag);

```