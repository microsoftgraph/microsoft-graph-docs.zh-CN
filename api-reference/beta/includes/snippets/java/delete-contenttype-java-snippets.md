---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 459470616fa6b39f0edcd90c2638db46222cf0129b830209261802ded6bdf1a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220913"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .delete();

```