---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c325560d7ced96e2614f904417cde8248f0d73f6709131c8c226cf827c2e1bc0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163513"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleDeltaCollectionPage delta = graphClient.directoryRoles()
    .delta()
    .buildRequest()
    .get();

```