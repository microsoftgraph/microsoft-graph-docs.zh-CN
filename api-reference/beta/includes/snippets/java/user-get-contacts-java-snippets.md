---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee2422f839c6c4971b3c63ea53ef7a7d17cadb58a736728fb76c72f8786d94ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactCollectionPage contacts = graphClient.me().contacts()
    .buildRequest()
    .select("displayName,emailAddresses")
    .get();

```