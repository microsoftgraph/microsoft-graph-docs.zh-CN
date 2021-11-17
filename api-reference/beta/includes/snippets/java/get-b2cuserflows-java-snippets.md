---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c977eb40ef48c027d5e17d7e8fde7091746ce0db20316f07368efda2b656f2ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .get();

```