---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2228ca8b5473b4ab012fae12f163c1bdd538f9f8f25fdf209b371c218370c37f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}")
    .buildRequest()
    .delete();

```