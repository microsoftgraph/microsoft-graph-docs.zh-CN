---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64374639403b68e1ae72c9c2deb8c89d2ad498db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .delete();

```