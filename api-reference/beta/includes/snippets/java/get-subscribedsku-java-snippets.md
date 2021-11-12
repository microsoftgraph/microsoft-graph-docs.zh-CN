---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: feee6d95417d5dc7c2af7743bbdfa4832a4a8a4656db18fe4e8d45e1dfdeb615
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscribedSku subscribedSku = graphClient.subscribedSkus("{id}")
    .buildRequest()
    .get();

```