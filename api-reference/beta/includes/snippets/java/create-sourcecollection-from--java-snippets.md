---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 163e1ac83ec86073bf28316ef29c74b7e3dad0ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978095"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.displayName = "Quarterly Financials search";
sourceCollection.contentQuery = "subject:'Quarterly Financials'";
sourceCollection.additionalDataManager().put("custodianSources@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735\"]"));

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections()
    .buildRequest()
    .post(sourceCollection);

```