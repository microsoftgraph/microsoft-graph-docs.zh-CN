---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1857fab19e5502c8761a36daae55f46796b7f1af
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522713"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda")
    .buildRequest()
    .get();

```