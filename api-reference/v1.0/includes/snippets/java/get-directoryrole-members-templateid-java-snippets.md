---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c948ddc9f047c72337a51171c3687ab1e9a668b5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf").members()
    .buildRequest()
    .get();

```