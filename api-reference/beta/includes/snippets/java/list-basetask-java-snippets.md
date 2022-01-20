---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac57c7b2d3817170e86e14738b7b6a05c1e211c2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114158"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskCollectionPage tasks = graphClient.me().tasks().lists("AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm").tasks()
    .buildRequest()
    .get();

```