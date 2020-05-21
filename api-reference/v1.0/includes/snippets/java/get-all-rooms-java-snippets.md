---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 939d03cd65fc04d196f5c166d42d2a18d1a7bc1d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334624"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomCollectionPage microsoft.graph.room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```