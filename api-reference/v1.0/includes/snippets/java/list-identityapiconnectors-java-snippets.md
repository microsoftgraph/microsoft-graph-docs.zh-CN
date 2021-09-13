---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f2c3ec4988a0edf96c6687dcfa6d05d318ec27a81e4d18ea9368ee3f98ed90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333935"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnectorCollectionPage apiConnectors = graphClient.identity().apiConnectors()
    .buildRequest()
    .get();

```