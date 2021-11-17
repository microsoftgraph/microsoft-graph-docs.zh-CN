---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14f27c081d528392ac8c44768706620a5d420da75bfdd00bfcac862eeea0121c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Onenote.Pages["{onenotePage-id}"]
    .Request()
    .DeleteAsync();

```