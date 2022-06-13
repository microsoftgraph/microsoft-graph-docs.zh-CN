---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c40f8de62c5891a08240c1431552cca4a0d27184
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id1}").members("{id2}").reference()
    .buildRequest()
    .delete();

```