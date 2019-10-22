---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e69df5584684bbc0baf3aeb8112a14206d39b87
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35890625"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.subscriptions("{id}")
    .buildRequest()
    .delete();

```