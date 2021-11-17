---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b4fec152899634790a5ce0914c2dded904eebdb84468dda1b96f5225cda4dc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsProtectionState windowsProtectionState = graphClient.tenantRelationships().managedTenants().windowsProtectionStates("{windowsProtectionStateId}")
    .buildRequest()
    .get();

```