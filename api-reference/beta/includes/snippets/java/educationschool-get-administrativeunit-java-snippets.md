---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee81bba1f7d60bae206e6d0b47691224c6d241db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955608"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.education().schools("2961761D-8094-4183-A9F6-8E36E966C7D9").administrativeUnit()
    .buildRequest()
    .get();

```