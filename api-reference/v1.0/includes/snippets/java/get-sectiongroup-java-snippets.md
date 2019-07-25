---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 306d67f6701ca12f0b04512edca43838fca4d952
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = graphClient.me().onenote().sectionGroups("{id}")
    .buildRequest()
    .get();

```