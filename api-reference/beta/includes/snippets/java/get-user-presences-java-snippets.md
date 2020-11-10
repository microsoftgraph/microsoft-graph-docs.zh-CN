---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 030ac9e6a209b27af15bbf5ca16af8e47fda112d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967129"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.communications().presences("dc74d9bb-6afe-433d-8eaa-e39d80d3a647")
    .buildRequest()
    .get();

```