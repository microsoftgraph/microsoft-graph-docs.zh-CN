---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c56eecd851af300cc82dd4dc25609ab1365922dcbf6454a19d850fa9346cc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b")
    .buildRequest()
    .get();

```