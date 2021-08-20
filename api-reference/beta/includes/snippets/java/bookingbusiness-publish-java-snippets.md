---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5b5f4a1ec3fb4ee09e199a46b41ba0485d2d2d91f360b9e966498d721ea4d3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903132"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com")
    .publish()
    .buildRequest()
    .post();

```