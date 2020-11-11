---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f1edcf97a664083a8f6f19db744f62ee707651
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984080"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionWithReferencesPage followedSites = graphClient.me().followedSites()
    .buildRequest()
    .get();

```