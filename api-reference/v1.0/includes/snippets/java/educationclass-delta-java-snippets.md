---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42bc323e9d49c86fea7ef16c7dbdf856c8f44d8e
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassDeltaCollectionPage delta = graphClient.education().classes()
    .delta()
    .buildRequest()
    .get();

```