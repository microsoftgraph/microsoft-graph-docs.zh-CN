---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 742c62f95e928f3117ba3d92ec055b7ae777614f8d7703dfdb284dcb3b1924fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = graphClient.identity().userFlowAttributes("{id}")
    .buildRequest()
    .get();

```