---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3554618d58ddd5a1ef3bc5fcb0e3a50ffec213ea82b3a165a07ccece32eb2de1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278364"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```