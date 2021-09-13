---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dd49116a5143ea50bb1f22c97957a4f97407ce9a86f31c5f47d9cdce2119b16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserActivityRecentCollectionPage recent = graphClient.me().activities()
    .recent()
    .buildRequest()
    .get();

```