---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 615d21798011aa7b3a1909e966391d20caa619ecf95d9c04529244582b35ee87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162803"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = graphClient.me().profile().addresses("{id}")
    .buildRequest()
    .get();

```