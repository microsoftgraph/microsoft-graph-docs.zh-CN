---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000339ddcdfc70ac6cce699f85f00db5e6ac59d6847d047557c8831fac2597de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnectorCollectionPage connectors = graphClient.print().connectors()
    .buildRequest()
    .get();

```