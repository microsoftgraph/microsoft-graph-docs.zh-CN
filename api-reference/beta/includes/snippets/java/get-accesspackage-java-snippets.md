---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bf8d14f687169315c41cc61d3c48a9df2b234bcdd474ae914cf22277eefd58f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}")
    .buildRequest()
    .get();

```