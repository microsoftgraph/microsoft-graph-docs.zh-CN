---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce0c6fe1e0a034e0f0afb9b0cb043c0c12f52b7a417e7068ccb1791f10f9b5ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220813"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSourceCollectionWithReferencesPage custodianSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").custodianSources()
    .buildRequest()
    .get();

```