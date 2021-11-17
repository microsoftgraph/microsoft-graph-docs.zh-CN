---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3728eb90c6a5d75767861f7d1dce2c16ce9974491ef26adc3caec81cc2650e17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.MasterCategories["{outlookCategory-id}"]
    .Request()
    .DeleteAsync();

```