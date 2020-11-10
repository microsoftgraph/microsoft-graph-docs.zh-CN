---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306d67f6701ca12f0b04512edca43838fca4d952
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978997"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = graphClient.me().onenote().sectionGroups("{id}")
    .buildRequest()
    .get();

```