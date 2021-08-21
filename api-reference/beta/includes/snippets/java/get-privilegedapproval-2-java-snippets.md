---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a61e1c16c631106bf4a4f4f37271d7faad5b28a58759aa4b9e003035e612cec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218461"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApprovalCollectionPage privilegedApproval = graphClient.privilegedApproval()
    .buildRequest()
    .get();

```