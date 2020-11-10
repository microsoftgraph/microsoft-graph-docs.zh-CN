---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c450f051779918551dba474c2c366c809e153ac7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982076"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = new OnenoteSection();
onenoteSection.displayName = "Section name";

graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .post(onenoteSection);

```