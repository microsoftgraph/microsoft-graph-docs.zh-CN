---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56d7fc5f6b8264b1b3690de4c2b64a8b7e36c6df9c3fdc4a05850e79236e5294
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409805"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().termsOfUse().agreements("093b947f-8363-4979-a47d-4c52b33ee1be")
    .buildRequest()
    .delete();

```