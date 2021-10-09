---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9854d86194dded8f6d708cd94edac76e3dbc8b71c4b8bed64f3a68d562bd8a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220705"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredUsers = graphClient.devices("{id}").registeredUsers()
    .buildRequest()
    .get();

```