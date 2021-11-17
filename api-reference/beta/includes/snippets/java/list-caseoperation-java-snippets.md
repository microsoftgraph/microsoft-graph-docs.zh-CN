---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8de9df1fdd7b8ff6baa3400edc5e41ebb09b48413e919434bfbe7dbd2f4d648b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseOperationCollectionPage operations = graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583").operations()
    .buildRequest()
    .get();

```