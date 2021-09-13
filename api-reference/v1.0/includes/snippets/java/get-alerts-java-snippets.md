---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b81dd0758e2eb091da04d845d8266c22a6777c81cb06e8dfb25b4cb17faf8c4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AlertCollectionPage alerts = graphClient.security().alerts()
    .buildRequest()
    .get();

```