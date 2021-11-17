---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a869ca8829c0e30d05f619ca66774e37b9c1b9801c11937ef556304db099884
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Request()
    .DeleteAsync();

```