---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2610e64db6ae3c395f88c14b2b8cfc9a55f1762a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskDeltaCollectionPage delta = graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=").tasks()
    .delta()
    .buildRequest()
    .get();

```