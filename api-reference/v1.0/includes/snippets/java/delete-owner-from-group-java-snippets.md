---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d8bbda270ecc89f6ac16c5b76070f2ebb3a65bc
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35890729"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```