---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d16fe48debf999fac30bdc1cd2684b581add0bb3947e6f511a864fc73fc54f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163090"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProvisioningObjectSummaryCollectionPage provisioning = graphClient.auditLogs().provisioning()
    .buildRequest()
    .get();

```