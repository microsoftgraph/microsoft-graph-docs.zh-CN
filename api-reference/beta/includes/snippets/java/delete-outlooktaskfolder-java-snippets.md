---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dabe731aa8cb947e9f853ad99f35f12f9f08a5e0af4909f6f41f78f1e42fbeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903506"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPXAAA=")
    .buildRequest()
    .delete();

```