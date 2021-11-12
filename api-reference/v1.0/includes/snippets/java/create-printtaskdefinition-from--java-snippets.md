---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc1b100e59eef460e7f5d6c56266fd40fdb4391efd6e0e38de76fa0ce0183966
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161605"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = new PrintTaskDefinition();
printTaskDefinition.displayName = "Test TaskDefinitionName";
AppIdentity createdBy = new AppIdentity();
createdBy.displayName = "Requesting App Display Name";
printTaskDefinition.createdBy = createdBy;

graphClient.print().taskDefinitions()
    .buildRequest()
    .post(printTaskDefinition);

```