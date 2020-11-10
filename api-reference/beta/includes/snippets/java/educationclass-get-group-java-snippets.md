---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 961cabe2ca150fcd9b2da4a2f7fe04c86f5799ec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966320"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.education().classes("2961761D-8094-4183-A9F6-8E36E966C7D9").group()
    .buildRequest()
    .get();

```