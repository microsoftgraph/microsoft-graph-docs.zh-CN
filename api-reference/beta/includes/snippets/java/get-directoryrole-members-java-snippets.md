---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdebfa159fcd67383e9ceac1617a621f52afb5a2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda").members()
    .buildRequest()
    .get();

```