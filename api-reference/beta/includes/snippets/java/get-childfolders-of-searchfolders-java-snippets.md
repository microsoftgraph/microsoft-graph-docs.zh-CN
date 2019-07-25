---
description: 自动生成的文件。 不修改
ms.openlocfilehash: daba38f45260b401e2d8eba3da39ca532b34d1b6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880048"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage childFolders = graphClient.me().mailFolders("searchfolders").childFolders()
    .buildRequest()
    .get();

```