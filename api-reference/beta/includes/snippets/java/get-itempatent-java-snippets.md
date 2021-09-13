---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df2083cee201863b688cab5daf71bfa122e973bf1112e688bc37dff2742f8c3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = graphClient.me().profile().patents("{id}")
    .buildRequest()
    .get();

```