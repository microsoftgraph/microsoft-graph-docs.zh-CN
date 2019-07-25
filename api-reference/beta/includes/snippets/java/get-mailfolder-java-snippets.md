---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00b5775d6efbc9fbbd2a26bbe651cfd365d31d1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880090"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .get();

```