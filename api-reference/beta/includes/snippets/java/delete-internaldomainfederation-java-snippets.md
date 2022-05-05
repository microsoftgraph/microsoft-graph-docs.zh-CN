---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 496340b1a97ffe3281d5af5ec090c215d0b0b484
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com").federationConfiguration("96db02e2-80c1-5555-bc3a-de92ffb8c5be")
    .buildRequest()
    .delete();

```