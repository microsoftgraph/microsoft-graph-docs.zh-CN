---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9f32abefa65dba0056d6a98e16d3663b8214deb4d8e2b235574ff58b042f494
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105838"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointmentCollectionPage appointments = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments()
    .buildRequest()
    .get();

```