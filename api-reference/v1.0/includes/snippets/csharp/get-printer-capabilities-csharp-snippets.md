---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c98b94d8f7a9d93b704326b1a986ca7f074ec01690f8381bf785812e53bf4ef5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .Select("id,displayName,capabilities")
    .GetAsync();

```