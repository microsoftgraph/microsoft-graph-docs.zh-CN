---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ab8df03059d15a45340af56d8d4ff6f353c91797b099bd0f79e573a0fd90398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162105"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com")
    .unpublish()
    .buildRequest()
    .post();

```