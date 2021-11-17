---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cdea1dca6a7b1a80998c423b1995dfa89a7043ff9804a92bc6f5c9c5e509026
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274361"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .offboardTenant()
    .buildRequest()
    .post();

```