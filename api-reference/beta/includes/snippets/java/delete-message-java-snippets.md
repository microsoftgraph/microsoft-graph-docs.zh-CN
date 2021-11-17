---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2890072a75bb2d01f329e8cbbc37f4d5510bd402f0ece3fc3cf2b1c963f0f201
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163683"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .buildRequest()
    .delete();

```