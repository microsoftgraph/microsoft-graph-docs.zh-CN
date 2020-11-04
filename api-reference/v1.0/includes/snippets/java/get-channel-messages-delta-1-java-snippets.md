---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 474948b327791e491c21964b15a6bd218a8765f3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905015"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("{id}").channels("{id}").messages("delta")
    .buildRequest()
    .top(2)
    .get();

```