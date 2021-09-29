---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de81d8f046988d7e737e3962b0767cd4de3309defe58d5008deb2c83da4fd19f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106168"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = new NoncustodialDataSource();
noncustodialDataSource.additionalDataManager().put("@odata.id", new JsonPrimitive("https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"));

graphClient.compliance().ediscovery().cases("06d52284-ed81-49b8-904a-b863d3164731").sourceCollections("12aab1671c834213a84ba219c06f4c5a").noncustodialSources().references()
    .buildRequest()
    .post(noncustodialDataSource);

```