---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c99a119d1e57366487297ec723dec715b31c247
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210286"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DocumentSetVersion documentSetVersion = graphClient.sites("root").lists("Documents").items("2").documentSetVersions("1")
    .buildRequest()
    .get();

```