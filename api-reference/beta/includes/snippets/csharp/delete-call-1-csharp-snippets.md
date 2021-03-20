---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80311ccb656ae9901418312ee2011d5a62d9905e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"]
    .Request()
    .DeleteAsync();

```