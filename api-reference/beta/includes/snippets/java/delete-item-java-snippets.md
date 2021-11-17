---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebc255f00f2e04d81f5371b5c988e207e423b7914035e6710a104d833a610bc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest()
    .delete();

```