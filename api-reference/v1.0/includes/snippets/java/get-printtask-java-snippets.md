---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cebfe985789dcc35e4f763c59d43deaf01088dceffce9530d1af4bff00778557
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = graphClient.print().taskDefinitions("{taskDefinitionId}").tasks("{taskId}")
    .buildRequest()
    .get();

```