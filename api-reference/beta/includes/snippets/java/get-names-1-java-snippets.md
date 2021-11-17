---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 242717fd1930abae1354adf7554a5f8cdffa1b584659e0a0774bd6e986998775
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279633"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonNameCollectionPage names = graphClient.me().profile().names()
    .buildRequest()
    .get();

```