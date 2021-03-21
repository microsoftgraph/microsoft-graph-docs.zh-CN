---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a61976a490b273f854cc336a89a93c81b16c5e44
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978445"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocation namedLocation = graphClient.identity().conditionalAccess().namedLocations("0854951d-5fc0-4eb1-b392-9b2c9d7949c2")
    .buildRequest()
    .get();

```