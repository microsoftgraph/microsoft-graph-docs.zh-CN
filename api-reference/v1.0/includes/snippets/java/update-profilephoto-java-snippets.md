---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a18728e50059a7718d18eab4b87d9ea00fca141f072b034d00c248cad5cf997
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("Binary data for the image");
    graphClient.me().photo().content()
    .buildRequest()
    .put(stream);

```