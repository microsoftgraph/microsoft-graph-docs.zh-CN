---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7c76dc75d278d9d1fc47aa5e2510ddd77cc1bdc
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475374"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionPage users = graphClient.education().users()
    .buildRequest()
    .get();

```