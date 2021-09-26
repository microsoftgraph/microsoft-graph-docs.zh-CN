---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e44e078f53efb54293426dd0173c3e97e14514188146b63199069d55a4e25ec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162535"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.subscriptions("{id}")
    .buildRequest()
    .get();

```