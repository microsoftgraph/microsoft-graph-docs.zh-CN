---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0011fc93e69e6185f0897336fc1e049cf40d7bae33d519412747a3d1c0b2377f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("{id}")
    .buildRequest()
    .delete();

```