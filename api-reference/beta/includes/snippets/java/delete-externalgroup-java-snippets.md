---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 936cb43e43567c9d973c9a1baf343988b6964c2c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954647"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000")
    .buildRequest()
    .delete();

```