---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40338270a886b0546ae61a01f0e68885b6b21d7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").events()
    .buildRequest()
    .get();

```