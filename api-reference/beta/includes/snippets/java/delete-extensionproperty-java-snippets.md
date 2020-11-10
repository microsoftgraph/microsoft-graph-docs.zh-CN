---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b21daee4f26ade9832d7555e3f63eb7829d24073
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962260"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").extensionProperties("{id}")
    .buildRequest()
    .delete();

```