---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6851dfcfec58934c756ec4806aadfd1be7a7225e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968370"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("{role-objectId}").members("{user-id}").reference()
    .buildRequest()
    .delete();

```