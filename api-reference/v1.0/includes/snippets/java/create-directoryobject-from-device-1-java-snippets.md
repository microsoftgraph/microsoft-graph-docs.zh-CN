---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1c1852ec551b55186bf617a00b05784f751b73e5b4ee37e5f2bdf4e6a44db5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.devices("{id}").registeredOwners().references()
    .buildRequest()
    .post(directoryObject);

```