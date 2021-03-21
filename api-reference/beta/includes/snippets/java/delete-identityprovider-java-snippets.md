---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 538013f812c86efd46d34bdd1e46380dfe8445b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityProviders("{id}")
    .buildRequest()
    .delete();

```