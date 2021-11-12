---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07691174f5e0371fa7817d76c03cfa6a88288b376c79c1eae0570115b6b66193
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrency = await graphClient.BookingCurrencies["{bookingCurrency-id}"]
    .Request()
    .GetAsync();

```