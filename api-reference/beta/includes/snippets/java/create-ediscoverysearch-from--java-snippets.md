---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 305df3c04e9b4a374161b7d4d25468958e64b743
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoverySearch ediscoverySearch = new EdiscoverySearch();
ediscoverySearch.displayName = "My search 2";
ediscoverySearch.description = "My first search";
ediscoverySearch.contentQuery = "(Author=\"edison\")";
ediscoverySearch.additionalDataManager().put("custodianSources@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/43434642-3137-3138-3432-374142313639\",  \"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources/169718e3-a8df-449d-bef4-ee09fe1ddc5d\",  \"https://graph.microsoft.com/beta/security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')\"]"));
ediscoverySearch.additionalDataManager().put("noncustodialSources@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043\"]"));

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").searches()
    .buildRequest()
    .post(ediscoverySearch);

```