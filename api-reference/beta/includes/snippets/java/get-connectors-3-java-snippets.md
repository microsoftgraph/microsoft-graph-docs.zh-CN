---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f8bc11e938b2fb8c6f38118ded5e5224bfac717
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961471"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintConnectorCollectionWithReferencesPage connectors = graphClient.print().printers("{id}").connectors()
    .buildRequest()
    .get();

```