---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19c7a71007f1c246a862dc6c2ceebbb130a234f3bbdc05e945c00988fb3f4d05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .delete();

```