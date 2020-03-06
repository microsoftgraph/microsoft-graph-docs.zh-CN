---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b68ec07f7b8dcac374a56c8313e2aae48eda8636
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```