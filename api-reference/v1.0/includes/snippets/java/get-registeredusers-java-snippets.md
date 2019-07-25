---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 307e3385cfbf8954089af0861afd219ac83adaa9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883413"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage registeredUsers = graphClient.devices("{id}").registeredUsers()
    .buildRequest()
    .get();

```