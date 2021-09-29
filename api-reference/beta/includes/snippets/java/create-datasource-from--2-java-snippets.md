---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b0c1fde1b0c1776e2af29589fac193b2d323e49333e6546ebfff78ff6d0e5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSource dataSource = new DataSource();
dataSource.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119").custodianSources().references()
    .buildRequest()
    .post(dataSource);

```