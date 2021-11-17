---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9b893a55eadb887879bcad417918f2b382b1f9b8e9dfc6d765aaf679a14230e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = graphClient.bookingBusinesses("Fabrikam@M365B489948.onmicrosoft.com")
    .buildRequest()
    .get();

```