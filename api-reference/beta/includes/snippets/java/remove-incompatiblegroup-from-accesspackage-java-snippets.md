---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d58b5d5e40fe8fb7e9e113ce113589d9321b31f5a29acbe75753fa45f7d008c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104240"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleGroups("{id}").reference()
    .buildRequest()
    .delete();

```