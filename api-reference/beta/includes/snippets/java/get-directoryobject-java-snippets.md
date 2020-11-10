---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3963a132f94ba67766b15eb473d0c8fb2b030afe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963100"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("{id}")
    .buildRequest()
    .get();

```