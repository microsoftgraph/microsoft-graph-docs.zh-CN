---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42bc323e9d49c86fea7ef16c7dbdf856c8f44d8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978118"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassDeltaCollectionPage delta = graphClient.education().classes()
    .delta()
    .buildRequest()
    .get();

```