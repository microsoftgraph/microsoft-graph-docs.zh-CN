---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5e950f7d7a322e3b918be4c3cfadcb7573caf8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953475"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOpenShiftCollectionPage openShifts = graphClient.teams("{id}").schedule().openShifts()
    .buildRequest()
    .get();

```