---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cf694e70f86f6f1eb4050fe7225c50c60dbae7800219d59510ab9b01425aa9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .delete();

```