---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ca354fa1946e029a0e7b083bacd0a44e9067404
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877617"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPXAAA=")
    .buildRequest()
    .delete();

```