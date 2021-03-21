---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5ce5b792ab23a7815e7d7f3de7e242ea3f3d582
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978395"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredUsers = graphClient.devices("{id}").registeredUsers()
    .buildRequest()
    .get();

```