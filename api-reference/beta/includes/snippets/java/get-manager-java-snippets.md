---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2126825a47b97d1cf4d9c7dc82b77dc4c214e24b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524425"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.users("{id|userPrincipalName}").manager()
    .buildRequest()
    .get();

```