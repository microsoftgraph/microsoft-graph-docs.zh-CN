---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc4beaccdae032f1bd8024adcc98d3f638684a0b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.contacts("{id}").memberOf()
    .buildRequest()
    .get();

```