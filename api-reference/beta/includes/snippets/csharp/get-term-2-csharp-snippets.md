---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e54d8cd0be94130215cbf9e468e351198cdb3ea4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.TermStore.Sets["{termStore.set-id}"].Children
    .Request()
    .GetAsync();

```