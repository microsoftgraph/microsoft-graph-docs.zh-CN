---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f59331b8a018a1dcf869ae25c1277519c6337d84c50d871f69a09af6becb9f6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .GetAsync();

```