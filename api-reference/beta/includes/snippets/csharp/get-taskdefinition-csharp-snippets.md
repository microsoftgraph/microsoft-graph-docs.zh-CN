---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7902876d2428918ef7174d9e1725a8b1aa8eed4b058ec7c20b37b18146085900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"]
    .Request()
    .GetAsync();

```