---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8651bb7c343aa1d5f10396cf553df06268df7b38
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040843"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().administrativeUnits("c5729e7c-988e-417b-b287-14f5bd4711d8").members("7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac")
    .buildRequest()
    .get();

```