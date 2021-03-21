---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd73cc1d4200dff86d183f89fcafc964d1d9c102
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}")
    .buildRequest()
    .get();

```