---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e559f857ae2d2cd7bdae76b654914633f200a8a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").channels("{id}").members("{id}")
    .buildRequest()
    .delete();

```