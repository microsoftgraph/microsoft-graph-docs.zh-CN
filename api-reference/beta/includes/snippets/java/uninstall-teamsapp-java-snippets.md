---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beb5bdd405bb55b0a6f8ec3a2309defd1cf77cf7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967251"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .delete();

```