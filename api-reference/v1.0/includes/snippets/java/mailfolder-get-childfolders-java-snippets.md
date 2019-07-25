---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64e1cfcf503a8ac8940db1bae06e9d5190bf8970
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881373"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage childFolders = graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .get();

```