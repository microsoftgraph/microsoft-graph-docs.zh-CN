---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cfe3d55816e1c62dcf56b29c5b263e59f4ec9c5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097911"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleDefinitions("f189965f-f560-4c59-9101-933d4c87a91a")
    .buildRequest()
    .delete();

```