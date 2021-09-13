---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff70540b1e49e5b1067cd1e8372838db7c8c433676425bb27a36c0b5c859f3ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277678"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf")
    .buildRequest()
    .get();

```