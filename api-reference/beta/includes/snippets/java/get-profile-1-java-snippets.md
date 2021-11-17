---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b061b7b8f7a083500e133f0b3d28842f3b69bab033f94c1e644e0cd554e96afd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274140"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Profile profile = graphClient.me().profile()
    .buildRequest()
    .get();

```