---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b6f242235b57d5b9a9e43c183696e2f4420e82a
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSetCollectionPage attributeSets = graphClient.directory().attributeSets()
    .buildRequest()
    .get();

```