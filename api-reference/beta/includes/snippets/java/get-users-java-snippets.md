---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36c215da64333b7c3117788aabf8e22410b7bb06
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953773"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .get();

```