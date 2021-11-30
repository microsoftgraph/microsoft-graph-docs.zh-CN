---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23bbfbc5abe7c883f4322e9996e96a13d6040f12
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225506"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSetCollectionPage attributeSets = graphClient.directory().attributeSets()
    .buildRequest()
    .top(10)
    .get();

```