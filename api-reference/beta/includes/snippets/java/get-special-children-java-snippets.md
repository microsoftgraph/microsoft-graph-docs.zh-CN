---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 458884f4a36a18cd083aeda550e4ccb2f133d696
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().special("{name}").children()
    .buildRequest()
    .get();

```