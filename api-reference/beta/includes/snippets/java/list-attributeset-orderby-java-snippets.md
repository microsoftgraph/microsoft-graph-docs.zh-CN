---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a00b95511839757b889d12794e5b7d92d197b9ee
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225512"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSetCollectionPage attributeSets = graphClient.directory().attributeSets()
    .buildRequest()
    .orderBy("id")
    .get();

```