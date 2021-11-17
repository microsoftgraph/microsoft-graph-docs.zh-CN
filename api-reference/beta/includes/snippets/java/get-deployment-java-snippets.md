---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f94fb797b5ee9a0999466e8f1d4be26cdd52f7e49bcad9755d0f47a57d22f230
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903021"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Deployment deployment = graphClient.admin().windows().updates().deployments("b5171742-1742-b517-4217-17b5421717b5")
    .buildRequest()
    .get();

```