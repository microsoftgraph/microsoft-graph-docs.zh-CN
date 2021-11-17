---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee97329195f8707132d99a77d0c0fc405bc4e664
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61031754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().softwareOathMethods("b172893e-893e-b172-3e89-72b13e8972b1")
    .buildRequest()
    .delete();

```