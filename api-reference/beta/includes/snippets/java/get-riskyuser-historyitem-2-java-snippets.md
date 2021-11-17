---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6efef76e740ddc3e21356b64c446fdca20b8d5ed64543d20e78a9ac71b8843d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104747"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItem riskyUserHistoryItem = graphClient.identityProtection().riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69")
    .buildRequest()
    .get();

```