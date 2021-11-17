---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41003b7158e7bd61948198289019440f2b9d058c44b2496074ed80b3a8d94271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277794"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .get();

```