---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74844225afd836bea9145b444bd6e78e762a4dbc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960117"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendar()
    .buildRequest()
    .delete();

```