---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93a84877aa58ae6146b0584f24dfcfe4fd1f2ac17f76b35fba03615e3c29c70c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contract = await graphClient.Contracts["{contract-id}"]
    .Request()
    .GetAsync();

```