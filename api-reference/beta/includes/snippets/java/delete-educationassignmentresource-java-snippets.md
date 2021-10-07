---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8089d41e568898f31cd1054b2b2ae045fd8a1310e07a8cdc449bf25203fa3b18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220517"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").resources("22002")
    .buildRequest()
    .delete();

```