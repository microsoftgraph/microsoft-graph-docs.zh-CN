---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38c0aa938bb68d986ae740f75fcc42bcb6f7b7114e72d2c599d32bea040b5d8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104845"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors().references()
    .buildRequest()
    .post(directoryObject);

```