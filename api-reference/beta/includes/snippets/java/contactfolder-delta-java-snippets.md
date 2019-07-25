---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a35a6de412e3b5ed0c0e44b7ca2f2a223f61b00e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863374"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactFolderDeltaCollectionPage delta = graphClient.me().contactFolders()
    .delta()
    .buildRequest()
    .get();

```