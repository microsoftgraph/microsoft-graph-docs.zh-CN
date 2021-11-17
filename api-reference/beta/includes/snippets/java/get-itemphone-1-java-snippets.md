---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfea9ba5745494d9a3ad48752188224e8b4d1840c9fffa27c0db5224f73ae267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = graphClient.me().profile().phones("{id}")
    .buildRequest()
    .get();

```