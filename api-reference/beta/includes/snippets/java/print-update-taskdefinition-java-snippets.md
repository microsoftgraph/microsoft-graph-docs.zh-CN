---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca1d2dd00e894b7fbe1841987a4a250229dc27a444ec617e7db78a7d3f55c109
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278667"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = new PrintTaskDefinition();
printTaskDefinition.displayName = "Test TaskDefinitionName";
AppIdentity createdBy = new AppIdentity();
createdBy.displayName = "Requesting App Display Name";
printTaskDefinition.createdBy = createdBy;

graphClient.print().taskDefinitions("fab143fd-ee61-4358-8558-2c7dee953982")
    .buildRequest()
    .patch(printTaskDefinition);

```