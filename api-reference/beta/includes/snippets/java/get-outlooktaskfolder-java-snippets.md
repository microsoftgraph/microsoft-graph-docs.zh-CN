---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 419b519eeda22b93791102573e31a740ba148a98
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972809"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = graphClient.me().outlook().taskFolders("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```