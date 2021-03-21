---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdebfa159fcd67383e9ceac1617a621f52afb5a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978787"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda").members()
    .buildRequest()
    .get();

```