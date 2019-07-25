---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32114b75c9c60a940ed07399059e1d4cc08ebb7a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862070"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectorySettingCollectionPage settings = graphClient.settings()
    .buildRequest()
    .get();

```