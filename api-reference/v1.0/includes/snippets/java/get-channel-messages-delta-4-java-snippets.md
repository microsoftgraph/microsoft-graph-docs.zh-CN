---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a89b54967c6f585ce640f030db81e96cb37e63c1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("{id}").channels("{id}").messages("delta")
    .buildRequest()
    .get();

```