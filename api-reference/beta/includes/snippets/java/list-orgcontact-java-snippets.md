---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b490464b711176bdcb668bf3ffd22324e46afebfdccf4805dc75364b26cbd89f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```