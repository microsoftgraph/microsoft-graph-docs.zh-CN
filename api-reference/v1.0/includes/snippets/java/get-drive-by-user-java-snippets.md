---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3524c3d143bced8da2f9d094dbc8393bedd58fc2c917590649b425d0ffc957c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902313"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.users("{idOrUserPrincipalName}").drive()
    .buildRequest()
    .get();

```