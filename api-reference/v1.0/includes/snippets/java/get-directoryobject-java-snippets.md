---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3963a132f94ba67766b15eb473d0c8fb2b030afe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882741"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("{id}")
    .buildRequest()
    .get();

```