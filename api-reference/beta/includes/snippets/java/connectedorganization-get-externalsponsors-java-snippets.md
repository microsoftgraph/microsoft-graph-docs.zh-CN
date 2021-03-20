---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fb5de73e4fb8907d8834dba623296f7de6e7f44
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage externalSponsors = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors()
    .buildRequest()
    .get();

```