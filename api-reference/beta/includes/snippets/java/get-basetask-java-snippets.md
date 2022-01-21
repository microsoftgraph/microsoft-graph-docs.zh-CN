---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97418a33323d1d5349a0e104b4fdd976d0bce371
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109784"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTask baseTask = graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA")
    .buildRequest()
    .get();

```