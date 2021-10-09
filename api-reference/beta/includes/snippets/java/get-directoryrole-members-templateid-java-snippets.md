---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55264a3b3ed17fecc7105578e3aa5b951dd7ff3eac1401c955ab366bd8c68cf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf").members()
    .buildRequest()
    .get();

```