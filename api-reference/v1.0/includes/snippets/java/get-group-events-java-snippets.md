---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86b1a333770bfb61f92ef52aaae2d69ef11fa23336f3b6f8878d0a9b017b228f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107042"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").events()
    .buildRequest()
    .get();

```