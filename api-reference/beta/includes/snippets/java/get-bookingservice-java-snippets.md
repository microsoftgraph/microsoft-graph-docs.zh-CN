---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05b776e6a95d33896f3cbe4b074576bff0905b5a2a99db6c2b4da307449b3a0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .get();

```