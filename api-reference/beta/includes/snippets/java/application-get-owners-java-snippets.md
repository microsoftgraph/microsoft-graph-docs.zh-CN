---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 67a21f9447e399c0b2ba902ad59ea94844de239d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855249"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage owners = graphClient.applications("{id}").owners()
    .buildRequest()
    .get();

```