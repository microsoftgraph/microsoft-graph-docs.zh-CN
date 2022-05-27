---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b761ce6fbf4cca49d8325484bc3762c97947f2a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RichLongRunningOperationCollectionPage operations = graphClient.sites("root").operations()
    .buildRequest()
    .get();

```