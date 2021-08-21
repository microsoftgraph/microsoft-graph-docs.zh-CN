---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd46e7ecc0f1288eb29e150548aff9b1b904b893492ed5813ce5fab6c4f578e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignments("{id}")
    .makeEligible()
    .buildRequest()
    .post();

```