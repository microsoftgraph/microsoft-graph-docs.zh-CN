---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99fce0b870f2767230b095a3932a73c360adcbc0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979382"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderDeltaCollectionPage delta = graphClient.me().mailFolders()
    .delta()
    .buildRequest()
    .get();

```