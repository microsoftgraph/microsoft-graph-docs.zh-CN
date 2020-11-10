---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f945cff9a5d7c0b3d7346169a0e1d6ef2cf8f09
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971892"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("{id}")
    .buildRequest()
    .get();

```