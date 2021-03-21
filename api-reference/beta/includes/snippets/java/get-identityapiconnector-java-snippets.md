---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f339326f6e30976ab1125b3167101c205f873fde
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968765"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = graphClient.identity().apiConnectors("{id}")
    .buildRequest()
    .get();

```