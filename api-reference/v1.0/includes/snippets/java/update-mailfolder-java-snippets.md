---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66b2101ff7af4e2d42dd5c1557d95b520ae04a95
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856259"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders("{id}")
    .buildRequest()
    .patch(mailFolder);

```