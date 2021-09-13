---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cb2cd98f135ec8f7a8d9dc7840e662f01a368a33879b958f6aa957e333dddbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").defaultPages("idpselections").content()
    .buildRequest()
    .get();

```