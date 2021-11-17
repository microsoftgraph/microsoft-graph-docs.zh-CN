---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d08dc0fd984e548a83d7a1f2754bc016d944f710cdff371fb992c6c46e1bdc50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers("80b5ddda-1e3b-4c9d-abe2-d606cc075e2e")
    .buildRequest()
    .delete();

```