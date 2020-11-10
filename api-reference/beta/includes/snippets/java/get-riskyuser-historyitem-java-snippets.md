---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09d3be5971fcbcde9e249a352d55f4a84e7d924e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977610"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItem riskyUserHistoryItem = graphClient.identityProtection().riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69")
    .buildRequest()
    .get();

```