---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d824175e32957c3846b5c95796e22a051b6d948
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969435"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.programControls("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .delete();

```