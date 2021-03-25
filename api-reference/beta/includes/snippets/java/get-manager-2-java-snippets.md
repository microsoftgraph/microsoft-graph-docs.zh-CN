---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab7d8d03bd6be97ffdbf7e429847c6fc14895006
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.users("{id|userPrincipalName}").manager()
    .buildRequest()
    .get();

```