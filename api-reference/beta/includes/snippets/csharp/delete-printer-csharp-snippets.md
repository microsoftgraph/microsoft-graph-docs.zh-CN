---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc9df4af805fb26afc2169e287007de9d4b8ca1e8b198c0b0583e54c883a84b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .DeleteAsync();

```