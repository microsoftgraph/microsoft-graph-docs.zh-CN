---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed37a22245392ee7eb577586fdb979c856b29d4bc87573951b516f4a3b448dd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/onenote/resources/{id}/content", InputStream.class)
    .buildRequest()
    .get();

```