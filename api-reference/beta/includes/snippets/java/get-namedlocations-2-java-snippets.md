---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 070521edd521f4a039ce512977385e4636ae50fc
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .filter("isof('microsoft.graph.ipNamedLocation')")
    .get();

```