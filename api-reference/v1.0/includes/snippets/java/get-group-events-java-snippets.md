---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40b5842b6e49ea83ad8b7b228eadd26c20f39880
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889203"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEventCollectionPage events = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").events()
    .buildRequest()
    .get();

```