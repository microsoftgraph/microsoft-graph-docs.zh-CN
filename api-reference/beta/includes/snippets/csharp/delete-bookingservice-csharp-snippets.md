---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd33c8304632f8abbdcf2bdd95790762306aa0019834546c1b4b1a989a4dd753
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services["{bookingService-id}"]
    .Request()
    .DeleteAsync();

```