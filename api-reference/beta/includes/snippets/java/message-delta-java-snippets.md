---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ab8d9824727661245dd7935591a49d98c71d8ae
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879641"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageDeltaCollectionPage delta = graphClient.me().mailFolders("{id}").messages()
    .delta()
    .buildRequest()
    .get();

```