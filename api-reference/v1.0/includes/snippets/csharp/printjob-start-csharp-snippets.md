---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e71d35338dce9c153c2a241832c45432121d94fb7f1c903b06571eb4de4c4b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"].Jobs["{printJob-id}"]
    .Start()
    .Request()
    .PostAsync();

```