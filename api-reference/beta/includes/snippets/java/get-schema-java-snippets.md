---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81daa19e530a49b0f5c91fac3136fc5a94c6f9e6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975343"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = graphClient.external().connections("contosohr").schema()
    .buildRequest()
    .get();

```