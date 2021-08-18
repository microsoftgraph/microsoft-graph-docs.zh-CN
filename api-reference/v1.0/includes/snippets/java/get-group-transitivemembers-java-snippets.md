---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7eb8bea7ffb8735b26a3c80f8e9d274e74f177060323f582ff3833b10de5f87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328956"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMembers = graphClient.groups("{id}").transitiveMembers()
    .buildRequest()
    .get();

```