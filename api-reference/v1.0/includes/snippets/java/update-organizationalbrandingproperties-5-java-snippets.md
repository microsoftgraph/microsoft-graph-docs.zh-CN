---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaa2a135559e9883f4c5fb4cf94adda170d4e61d0052d2a94589b87f987975d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221407"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("<Image>");
    graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr")
    .buildRequest()
    .put(stream);

```