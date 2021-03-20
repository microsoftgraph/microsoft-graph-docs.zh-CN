---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3d22065dfab77b9b2a2227046e609835eadcd5c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADYAAAImV_jAAA=")
    .buildRequest()
    .expand("eventMessage/event")
    .get();

```