---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcf2198151379e30ecfff44c4760e1c0fe0cfc2aa5165f5468b7c3f4f3e325ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278973"
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