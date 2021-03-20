---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e5b2b5a0b54181e1c335800705b5f2b7e1f5a6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage internalSponsors = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").internalSponsors()
    .buildRequest()
    .get();

```