---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c0d9b566900d2e73fd7708766d62fc884b52f046b3bd8d28e883c6fbdfd1578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .delete();

```