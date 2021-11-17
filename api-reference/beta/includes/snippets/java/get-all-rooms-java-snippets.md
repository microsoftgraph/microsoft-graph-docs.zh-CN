---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0c7679a69fc09d274f4e546a156577b678cffb40fc81c3ca0231159a1420cfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220249"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomCollectionPage room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```