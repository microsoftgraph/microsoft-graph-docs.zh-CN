---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fae2a3163a01c093c626d181ae018aa0395f7ac11310a8cc1315f4b8f277c8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.shares("{shareIdOrUrl}").driveItem()
    .buildRequest()
    .expand("children")
    .get();

```