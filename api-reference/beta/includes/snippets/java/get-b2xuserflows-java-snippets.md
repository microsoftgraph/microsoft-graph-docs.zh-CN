---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a6e4e62d5d47a38056b7e454df035fb9894b4b2168972b2d13fad8a8bd8a91b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903458"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = graphClient.identity().b2xUserFlows("{id}")
    .buildRequest()
    .get();

```