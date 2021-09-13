---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e95348fabd8033f3528b4f7f2a00d60f225e649445af24841c9bedf25ebb2363
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221416"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .restoreVersion()
    .buildRequest()
    .post();

```