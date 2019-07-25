---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87dac159e905c58a8b8df0957302da58874bb2e5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879838"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.mailSearchFolder"));
mailFolder.filterQuery = "contains(subject, 'Analytics')";

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .patch(mailFolder);

```