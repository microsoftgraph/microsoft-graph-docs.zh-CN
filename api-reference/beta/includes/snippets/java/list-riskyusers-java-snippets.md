---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 550bcfb2194ec1536f9ef0197899ab0bce6b960c842a8fb6e539eb3ded573ca7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104736"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserCollectionPage riskyUsers = graphClient.riskyUsers()
    .buildRequest()
    .get();

```