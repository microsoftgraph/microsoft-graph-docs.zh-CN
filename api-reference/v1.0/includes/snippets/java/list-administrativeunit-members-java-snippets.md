---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6cef51316c57a26600a2910799e0dce8819d3b
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040951"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directory().administrativeUnits("c5729e7c-988e-417b-b287-14f5bd4711d8").members()
    .buildRequest()
    .get();

```