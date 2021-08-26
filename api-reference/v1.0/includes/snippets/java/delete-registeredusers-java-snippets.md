---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d4fab6227c4b345e96c8296e7ccd84008e5cca3f3855e541f90a24c95d00e3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333528"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}").registeredUsers("{id}").reference()
    .buildRequest()
    .delete();

```