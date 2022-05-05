---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f0a21b696510cd6a6ab1bda08298b2148ba1dcb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DocumentSetVersionCollectionPage documentSetVersions = graphClient.sites("root").lists("Documents").items("1").documentSetVersions()
    .buildRequest()
    .get();

```