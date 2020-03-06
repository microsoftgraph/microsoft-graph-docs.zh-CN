---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d85c9248d40d33a3d8cc31a9053e027ea76c5d3e
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558948"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .get();

```