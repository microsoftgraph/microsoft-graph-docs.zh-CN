---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b098a2fe560d9123139d95ac44cfb628a6479b42f6baa9a8cd19fbb08f3cdcfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409328"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .get();

```