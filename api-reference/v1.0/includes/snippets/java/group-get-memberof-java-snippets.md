---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2d6c54e0bec892cb0a45ba6abc4d67eb0be5f0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.groups("{id}").memberOf()
    .buildRequest()
    .get();

```