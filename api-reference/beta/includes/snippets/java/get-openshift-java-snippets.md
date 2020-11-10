---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e950f7d7a322e3b918be4c3cfadcb7573caf8b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968748"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOpenShiftCollectionPage openShifts = graphClient.teams("{id}").schedule().openShifts()
    .buildRequest()
    .get();

```