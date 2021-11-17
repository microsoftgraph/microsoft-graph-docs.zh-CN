---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a5c4496f1b87769568098756ae014f04d5441bb789caa3ee76175698d389de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodCollectionPage methods = graphClient.me().authentication().methods()
    .buildRequest()
    .get();

```