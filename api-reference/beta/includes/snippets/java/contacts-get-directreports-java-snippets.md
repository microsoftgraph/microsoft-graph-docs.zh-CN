---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 039a80030d5bb6df1228db08140fc3fcd6c25f2f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877932"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage directReports = graphClient.contacts("{id}").directReports()
    .buildRequest()
    .get();

```