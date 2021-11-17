---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af35c3cbd05dd3ab9f2a4d7ccefed29dda341fb3036f4bc89e5ce1e8a701713a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda").members()
    .buildRequest()
    .get();

```