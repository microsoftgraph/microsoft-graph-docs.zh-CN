---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfdac6ca94e0c06a56fd87794379c87110bf233f79d436b0dd1868d722d5bd04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279246"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .invalidateAllRefreshTokens()
    .buildRequest()
    .post();

```