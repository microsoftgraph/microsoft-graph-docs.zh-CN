---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef0433d1fadb602c1466f87e7310e5c7879fde7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976834"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnenoteSectionCollectionPage sections = graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .get();

```