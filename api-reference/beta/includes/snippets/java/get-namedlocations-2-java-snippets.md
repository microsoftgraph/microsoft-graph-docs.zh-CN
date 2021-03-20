---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e160ebef0be54a2dd39f9ed68f1590a1372985af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947411"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

INamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .filter("isof('microsoft.graph.ipNamedLocation')")
    .get();

```