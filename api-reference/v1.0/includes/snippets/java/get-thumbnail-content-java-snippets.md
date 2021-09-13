---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0a89d1f735c8d01c164869bd5e05e0ec31e432cc3de08dc9361dd3908f0861b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333803"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content content = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}().content()
    .buildRequest()
    .get();

```